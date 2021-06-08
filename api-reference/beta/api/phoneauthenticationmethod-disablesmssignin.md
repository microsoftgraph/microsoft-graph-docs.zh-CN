---
title: phoneAuthenticationMethod：disableSmsSignIn
description: 禁用短信手机登录
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 00141db043825d96611eaae156adb2bbf2e48503
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786467"
---
# <a name="phoneauthenticationmethod-disablesmssignin"></a><span data-ttu-id="ca254-103">phoneAuthenticationMethod：disableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="ca254-103">phoneAuthenticationMethod: disableSmsSignIn</span></span>

<span data-ttu-id="ca254-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca254-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca254-105">禁用短信电话号码的 `mobile` 登录。</span><span class="sxs-lookup"><span data-stu-id="ca254-105">Disable SMS sign-in for an existing `mobile` phone number.</span></span> 

><span data-ttu-id="ca254-106">**注意：** 此号码将不再可用于短信登录，从而可能阻止用户登录。</span><span class="sxs-lookup"><span data-stu-id="ca254-106">**Note:** The number will no longer be available for SMS sign-in, which can prevent your user from signing in.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca254-107">权限</span><span class="sxs-lookup"><span data-stu-id="ca254-107">Permissions</span></span>

<span data-ttu-id="ca254-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca254-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="ca254-110">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="ca254-110">Permissions acting on self</span></span>

|<span data-ttu-id="ca254-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca254-111">Permission type</span></span>      | <span data-ttu-id="ca254-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca254-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="ca254-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca254-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca254-114">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca254-114">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="ca254-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca254-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca254-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca254-116">Not supported.</span></span> |
| <span data-ttu-id="ca254-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca254-117">Application</span></span>                            | <span data-ttu-id="ca254-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca254-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="ca254-119">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="ca254-119">Permissions acting on other users</span></span>

|<span data-ttu-id="ca254-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca254-120">Permission type</span></span>      | <span data-ttu-id="ca254-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca254-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="ca254-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca254-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca254-123">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca254-123">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="ca254-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca254-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca254-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca254-125">Not supported.</span></span> |
| <span data-ttu-id="ca254-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca254-126">Application</span></span>                            | <span data-ttu-id="ca254-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca254-127">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="ca254-128">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="ca254-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="ca254-129">全局管理员</span><span class="sxs-lookup"><span data-stu-id="ca254-129">Global admin</span></span>
* <span data-ttu-id="ca254-130">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="ca254-130">Privileged authentication admin</span></span>
* <span data-ttu-id="ca254-131">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="ca254-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="ca254-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca254-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/disableSmsSignIn
POST /users/{id | userPrincipalName}/authentication/phoneMethods/{id}/disableSmsSignIn
```
<span data-ttu-id="ca254-133">`id`phoneType 的 `mobile` 值为 `3179e48a-750b-4051-897c-87b9720928f7` 。</span><span class="sxs-lookup"><span data-stu-id="ca254-133">The value of `id` for the `mobile` phoneType is `3179e48a-750b-4051-897c-87b9720928f7`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca254-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca254-134">Request headers</span></span>

| <span data-ttu-id="ca254-135">名称</span><span class="sxs-lookup"><span data-stu-id="ca254-135">Name</span></span>          | <span data-ttu-id="ca254-136">说明</span><span class="sxs-lookup"><span data-stu-id="ca254-136">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ca254-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca254-137">Authorization</span></span> | <span data-ttu-id="ca254-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca254-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca254-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca254-140">Request body</span></span>

<span data-ttu-id="ca254-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ca254-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca254-142">响应</span><span class="sxs-lookup"><span data-stu-id="ca254-142">Response</span></span>

<span data-ttu-id="ca254-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ca254-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ca254-145">示例</span><span class="sxs-lookup"><span data-stu-id="ca254-145">Examples</span></span>

<span data-ttu-id="ca254-146">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="ca254-146">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="ca254-147">请求</span><span class="sxs-lookup"><span data-stu-id="ca254-147">Request</span></span>

<span data-ttu-id="ca254-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ca254-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ca254-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca254-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_disablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/disableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="ca254-150">C#</span><span class="sxs-lookup"><span data-stu-id="ca254-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-disablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca254-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca254-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-disablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca254-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca254-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-disablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca254-153">Java</span><span class="sxs-lookup"><span data-stu-id="ca254-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/phoneauthenticationmethod-disablesmssignin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ca254-154">响应</span><span class="sxs-lookup"><span data-stu-id="ca254-154">Response</span></span>

<span data-ttu-id="ca254-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ca254-155">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phoneAuthenticationMethod: disableSmsSignIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
