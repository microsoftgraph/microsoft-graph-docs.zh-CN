---
title: 创建 phoneAuthenticationMethod
description: 添加新的电话身份验证方法。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2bd29ee6e2f78e8864bce6a09cac456c4ab5ce6a
ms.sourcegitcommit: 4fa554d92a684d7720db1bd96befb9dea8d6ba5f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/30/2020
ms.locfileid: "44429582"
---
# <a name="create-phoneauthenticationmethod"></a><span data-ttu-id="296dd-103">创建 phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="296dd-103">Create phoneAuthenticationMethod</span></span>

<span data-ttu-id="296dd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="296dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="296dd-105">添加新的[电话身份验证方法](../resources/phoneauthenticationmethod.md)。</span><span class="sxs-lookup"><span data-stu-id="296dd-105">Add a new [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span> <span data-ttu-id="296dd-106">用户的每种类型只能有一个电话，在**phoneType**属性中捕获。</span><span class="sxs-lookup"><span data-stu-id="296dd-106">A user may only have one phone of each type, captured in the **phoneType** property.</span></span> <span data-ttu-id="296dd-107">这意味着， `mobile` 向具有预先存在的手机的用户添加电话将会 `mobile` 失败。</span><span class="sxs-lookup"><span data-stu-id="296dd-107">This means, for example, adding a `mobile` phone to a user with a preexisting `mobile` phone will fail.</span></span> <span data-ttu-id="296dd-108">此外，在添加电话之前，用户必须始终具有 `mobile` 电话 `alternateMobile` 。</span><span class="sxs-lookup"><span data-stu-id="296dd-108">Additionally, a user must always have a `mobile` phone before adding an `alternateMobile` phone.</span></span>

<span data-ttu-id="296dd-109">通过添加电话号码，可以在 Azure 多重身份验证（MFA）和自助服务密码重置（SSPR）（如果已启用）中使用。</span><span class="sxs-lookup"><span data-stu-id="296dd-109">Adding a phone number makes it available for use in both Azure multi-factor authentication (MFA) and self-service password reset (SSPR), if enabled.</span></span>

<span data-ttu-id="296dd-110">此外，如果用户启用了策略以使用 SMS 登录并添加了一个 `mobile` 号码，则系统会尝试注册该号码以在该系统中使用。</span><span class="sxs-lookup"><span data-stu-id="296dd-110">Additionally, if a user is enabled by policy to use SMS sign-in and a `mobile` number is added, the system will attempt to register the number for use in that system.</span></span>

## <a name="permissions"></a><span data-ttu-id="296dd-111">权限</span><span class="sxs-lookup"><span data-stu-id="296dd-111">Permissions</span></span>

<span data-ttu-id="296dd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="296dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="296dd-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="296dd-114">Permission type</span></span>                        | <span data-ttu-id="296dd-115">作用于自助的权限（从最高特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="296dd-115">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="296dd-116">对其他用户的权限（从最低到最高特权）</span><span class="sxs-lookup"><span data-stu-id="296dd-116">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="296dd-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="296dd-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="296dd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="296dd-118">Not supported.</span></span> | <span data-ttu-id="296dd-119">UserAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="296dd-119">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="296dd-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="296dd-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="296dd-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="296dd-121">Not supported.</span></span> | <span data-ttu-id="296dd-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="296dd-122">Not supported.</span></span> |
| <span data-ttu-id="296dd-123">Application</span><span class="sxs-lookup"><span data-stu-id="296dd-123">Application</span></span>                            | <span data-ttu-id="296dd-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="296dd-124">Not supported.</span></span> | <span data-ttu-id="296dd-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="296dd-125">Not supported.</span></span> |

<span data-ttu-id="296dd-126">对于在其他用户上执行管理的委派方案，管理员需要[以下角色之一](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="296dd-126">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="296dd-127">全局管理员</span><span class="sxs-lookup"><span data-stu-id="296dd-127">Global admin</span></span>
* <span data-ttu-id="296dd-128">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="296dd-128">Privileged authentication admin</span></span>
* <span data-ttu-id="296dd-129">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="296dd-129">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="296dd-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="296dd-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods
POST /users/{id}/authentication/phoneMethods
```

## <a name="request-headers"></a><span data-ttu-id="296dd-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="296dd-131">Request headers</span></span>

| <span data-ttu-id="296dd-132">名称</span><span class="sxs-lookup"><span data-stu-id="296dd-132">Name</span></span>          | <span data-ttu-id="296dd-133">说明</span><span class="sxs-lookup"><span data-stu-id="296dd-133">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="296dd-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="296dd-134">Authorization</span></span> | <span data-ttu-id="296dd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="296dd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="296dd-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="296dd-137">Content-Type</span></span>  | <span data-ttu-id="296dd-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="296dd-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="296dd-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="296dd-140">Request body</span></span>

<span data-ttu-id="296dd-141">在请求正文中，提供[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="296dd-141">In the request body, supply a JSON representation of a [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.</span></span> <span data-ttu-id="296dd-142">JSON 必须包括 `phoneNumber` and `phoneType` ，但不能 `smsSignInState` （只读）。</span><span class="sxs-lookup"><span data-stu-id="296dd-142">The JSON must include `phoneNumber` and `phoneType`, but not `smsSignInState` (which is read-only).</span></span>

| <span data-ttu-id="296dd-143">属性</span><span class="sxs-lookup"><span data-stu-id="296dd-143">Property</span></span>     | <span data-ttu-id="296dd-144">类型</span><span class="sxs-lookup"><span data-stu-id="296dd-144">Type</span></span>        | <span data-ttu-id="296dd-145">说明</span><span class="sxs-lookup"><span data-stu-id="296dd-145">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="296dd-146">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="296dd-146">phoneNumber</span></span>|<span data-ttu-id="296dd-147">String</span><span class="sxs-lookup"><span data-stu-id="296dd-147">String</span></span>|<span data-ttu-id="296dd-148">将电话号码设为文本或呼叫以进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="296dd-148">The phone number to text or call for authentication.</span></span> <span data-ttu-id="296dd-149">电话号码使用格式 "+ \<country code\> \<number\> x \<extension\> "，扩展名为可选。</span><span class="sxs-lookup"><span data-stu-id="296dd-149">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="296dd-150">例如，+ 1 5555551234 或 + 1 5555551234x123 是有效的。</span><span class="sxs-lookup"><span data-stu-id="296dd-150">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="296dd-151">如果创建/更新时编号不符合要求的格式，则会拒绝编号。</span><span class="sxs-lookup"><span data-stu-id="296dd-151">Numbers are rejected when creating/updating if they do not match the required format.</span></span>|
|<span data-ttu-id="296dd-152">phoneType</span><span class="sxs-lookup"><span data-stu-id="296dd-152">phoneType</span></span>|<span data-ttu-id="296dd-153">String</span><span class="sxs-lookup"><span data-stu-id="296dd-153">String</span></span>|<span data-ttu-id="296dd-154">可能的值为： `mobile` 、 `alternateMobile` 和 `office` 。</span><span class="sxs-lookup"><span data-stu-id="296dd-154">Possible values are: `mobile`, `alternateMobile`, and `office`.</span></span>|

## <a name="response"></a><span data-ttu-id="296dd-155">响应</span><span class="sxs-lookup"><span data-stu-id="296dd-155">Response</span></span>

<span data-ttu-id="296dd-156">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的[phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md)对象。</span><span class="sxs-lookup"><span data-stu-id="296dd-156">If successful, this method returns a `201 Created` response code and a new [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="296dd-157">示例</span><span class="sxs-lookup"><span data-stu-id="296dd-157">Examples</span></span>

### <a name="request"></a><span data-ttu-id="296dd-158">请求</span><span class="sxs-lookup"><span data-stu-id="296dd-158">Request</span></span>

<span data-ttu-id="296dd-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="296dd-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="296dd-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="296dd-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_phoneauthenticationmethod_from_authentication"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "mobile",
}
```
# <a name="c"></a>[<span data-ttu-id="296dd-161">C#</span><span class="sxs-lookup"><span data-stu-id="296dd-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-phoneauthenticationmethod-from-authentication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="296dd-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="296dd-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-phoneauthenticationmethod-from-authentication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="296dd-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="296dd-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-phoneauthenticationmethod-from-authentication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="296dd-164">响应</span><span class="sxs-lookup"><span data-stu-id="296dd-164">Response</span></span>

<span data-ttu-id="296dd-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="296dd-165">The following is an example of the response.</span></span>

> <span data-ttu-id="296dd-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="296dd-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
