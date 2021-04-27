---
title: 更新 phoneAuthenticationMethod
description: 更新与 phoneAuthenticationMethod 对象关联的电话号码。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5230ca00a63f3543b95ef4f2a1dc7242c5460a1b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055405"
---
# <a name="update-phoneauthenticationmethod"></a><span data-ttu-id="3cbb2-103">更新 phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3cbb2-103">Update phoneAuthenticationMethod</span></span>

<span data-ttu-id="3cbb2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cbb2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cbb2-105">更新与电话身份验证方法 [关联的电话号码](../resources/phoneauthenticationmethod.md)。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-105">Update the phone number associated with a [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span>

<span data-ttu-id="3cbb2-106">你无法更改电话的类型。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-106">You can't change a phone's type.</span></span> <span data-ttu-id="3cbb2-107">若要更改电话的类型，请添加所需类型的新号码，然后删除具有原始类型的对象。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-107">To change a phone's type, add a new number of the desired type and then delete the object with the original type.</span></span>

<span data-ttu-id="3cbb2-108">如果策略允许用户使用 短信登录并更改号码，系统将尝试注册号码以 `mobile` 用于该系统。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-108">If a user is enabled by policy to use SMS to sign in and the `mobile` number is changed, the system will attempt to register the number for use in that system.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cbb2-109">权限</span><span class="sxs-lookup"><span data-stu-id="3cbb2-109">Permissions</span></span>

<span data-ttu-id="3cbb2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="3cbb2-112">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="3cbb2-112">Permissions acting on self</span></span>

|<span data-ttu-id="3cbb2-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="3cbb2-113">Permission type</span></span>      | <span data-ttu-id="3cbb2-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3cbb2-114">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="3cbb2-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3cbb2-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="3cbb2-116">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3cbb2-116">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="3cbb2-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3cbb2-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cbb2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-118">Not supported.</span></span> |
| <span data-ttu-id="3cbb2-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="3cbb2-119">Application</span></span>                            | <span data-ttu-id="3cbb2-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-120">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="3cbb2-121">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="3cbb2-121">Permissions acting on other users</span></span>

|<span data-ttu-id="3cbb2-122">权限类型</span><span class="sxs-lookup"><span data-stu-id="3cbb2-122">Permission type</span></span>      | <span data-ttu-id="3cbb2-123">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3cbb2-123">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="3cbb2-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3cbb2-124">Delegated (work or school account)</span></span>     | <span data-ttu-id="3cbb2-125">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cbb2-125">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="3cbb2-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3cbb2-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cbb2-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-127">Not supported.</span></span> |
| <span data-ttu-id="3cbb2-128">应用程序</span><span class="sxs-lookup"><span data-stu-id="3cbb2-128">Application</span></span>                            | <span data-ttu-id="3cbb2-129">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cbb2-129">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="3cbb2-130">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="3cbb2-130">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="3cbb2-131">全局管理员</span><span class="sxs-lookup"><span data-stu-id="3cbb2-131">Global admin</span></span>
* <span data-ttu-id="3cbb2-132">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="3cbb2-132">Privileged authentication admin</span></span>
* <span data-ttu-id="3cbb2-133">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="3cbb2-133">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="3cbb2-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3cbb2-134">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/authentication/phoneMethods/{id}
PUT /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```
<span data-ttu-id="3cbb2-135">与要 `id` 更新的 phoneType 对应的值是下列值之一：</span><span class="sxs-lookup"><span data-stu-id="3cbb2-135">The value of `id` corresponding to the phoneType to update is one of the following:</span></span>
+ <span data-ttu-id="3cbb2-136">`b6332ec1-7057-4abe-9331-3d72feddfe41` 更新 `alternateMobile` **phoneType**。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-136">`b6332ec1-7057-4abe-9331-3d72feddfe41` to update the `alternateMobile` **phoneType**.</span></span>
+ <span data-ttu-id="3cbb2-137">`e37fc753-ff3b-4958-9484-eaa9425c82bc` 更新 `office` **phoneType**。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-137">`e37fc753-ff3b-4958-9484-eaa9425c82bc` to update the `office` **phoneType**.</span></span>
+ <span data-ttu-id="3cbb2-138">`3179e48a-750b-4051-897c-87b9720928f7` 更新 `mobile` **phoneType**。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-138">`3179e48a-750b-4051-897c-87b9720928f7` to update the `mobile` **phoneType**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cbb2-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="3cbb2-139">Request headers</span></span>

| <span data-ttu-id="3cbb2-140">名称</span><span class="sxs-lookup"><span data-stu-id="3cbb2-140">Name</span></span>       | <span data-ttu-id="3cbb2-141">说明</span><span class="sxs-lookup"><span data-stu-id="3cbb2-141">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3cbb2-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cbb2-142">Authorization</span></span> | <span data-ttu-id="3cbb2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3cbb2-145">Content-type</span><span class="sxs-lookup"><span data-stu-id="3cbb2-145">Content-type</span></span>  | <span data-ttu-id="3cbb2-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3cbb2-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3cbb2-148">请求正文</span><span class="sxs-lookup"><span data-stu-id="3cbb2-148">Request body</span></span>

<span data-ttu-id="3cbb2-149">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-149">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3cbb2-150">请求正文中未包含的现有属性将基于其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-150">Existing properties that are not included in the request body will be recalculated based on changes to other property values.</span></span>

| <span data-ttu-id="3cbb2-151">属性</span><span class="sxs-lookup"><span data-stu-id="3cbb2-151">Property</span></span>     | <span data-ttu-id="3cbb2-152">类型</span><span class="sxs-lookup"><span data-stu-id="3cbb2-152">Type</span></span>        | <span data-ttu-id="3cbb2-153">说明</span><span class="sxs-lookup"><span data-stu-id="3cbb2-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3cbb2-154">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="3cbb2-154">phoneNumber</span></span>|<span data-ttu-id="3cbb2-155">String</span><span class="sxs-lookup"><span data-stu-id="3cbb2-155">String</span></span>|<span data-ttu-id="3cbb2-156">要发送文本或呼叫进行身份验证的电话号码。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-156">The phone number to text or call for authentication.</span></span> <span data-ttu-id="3cbb2-157">电话数字使用格式"+ \<country code\> \<number\> \<extension\> x"，扩展是可选的。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-157">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="3cbb2-158">例如，+1 5555551234 或 +1 5555551234x123 有效。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-158">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="3cbb2-159">如果数字与所需格式不匹配，则创建/更新时将拒绝数字。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-159">Numbers are rejected when creating/updating if they do not match the required format.</span></span>|
|<span data-ttu-id="3cbb2-160">phoneType</span><span class="sxs-lookup"><span data-stu-id="3cbb2-160">phoneType</span></span>|<span data-ttu-id="3cbb2-161">string</span><span class="sxs-lookup"><span data-stu-id="3cbb2-161">string</span></span>| <span data-ttu-id="3cbb2-162">可能的值为： `mobile`、 `alternateMobile`或 `office`。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-162">Possible values are: `mobile`, `alternateMobile`, or `office`.</span></span>|

## <a name="response"></a><span data-ttu-id="3cbb2-163">响应</span><span class="sxs-lookup"><span data-stu-id="3cbb2-163">Response</span></span>

<span data-ttu-id="3cbb2-164">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-164">If successful, this method returns a `200 OK` response code and an updated [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3cbb2-165">示例</span><span class="sxs-lookup"><span data-stu-id="3cbb2-165">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3cbb2-166">请求</span><span class="sxs-lookup"><span data-stu-id="3cbb2-166">Request</span></span>

<span data-ttu-id="3cbb2-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3cbb2-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cbb2-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_phoneauthenticationmethod"
}-->

```http
PUT https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
Content-type: application/json

{
  "phoneNumber": "+1 2065555554",
  "phoneType": "mobile",
}
```
# <a name="c"></a>[<span data-ttu-id="3cbb2-169">C#</span><span class="sxs-lookup"><span data-stu-id="3cbb2-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cbb2-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cbb2-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cbb2-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cbb2-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cbb2-172">Java</span><span class="sxs-lookup"><span data-stu-id="3cbb2-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3cbb2-173">响应</span><span class="sxs-lookup"><span data-stu-id="3cbb2-173">Response</span></span>

<span data-ttu-id="3cbb2-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-174">The following is an example of the response.</span></span>

> <span data-ttu-id="3cbb2-175">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3cbb2-175">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "phoneNumber": "+1 2065555554",
  "phoneType": "mobile",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update phoneauthenticationmethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
