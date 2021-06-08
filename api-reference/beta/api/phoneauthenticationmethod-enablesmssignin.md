---
title: phoneAuthenticationMethod：enableSmsSignIn
description: 为短信启用登录。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1452d3e3e1c93def07dce3b6ee78a996c374ae0c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786466"
---
# <a name="phoneauthenticationmethod-enablesmssignin"></a><span data-ttu-id="cc603-103">phoneAuthenticationMethod：enableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="cc603-103">phoneAuthenticationMethod: enableSmsSignIn</span></span>

<span data-ttu-id="cc603-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc603-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc603-105">启用短信电话号码的登录 `mobile` 。</span><span class="sxs-lookup"><span data-stu-id="cc603-105">Enable SMS sign-in for an existing `mobile` phone number.</span></span> <span data-ttu-id="cc603-106">要成功启用：</span><span class="sxs-lookup"><span data-stu-id="cc603-106">To be successfully enabled:</span></span>

* <span data-ttu-id="cc603-107">手机必须具有 `"phoneType": "mobile"` 。</span><span class="sxs-lookup"><span data-stu-id="cc603-107">The phone must have `"phoneType": "mobile"`.</span></span>
* <span data-ttu-id="cc603-108">手机在登录短信必须是唯一 (其他人也不得使用该号码) 。</span><span class="sxs-lookup"><span data-stu-id="cc603-108">The phone must be unique in the SMS sign-in system (no one else can also be using that number).</span></span>
* <span data-ttu-id="cc603-109">必须在身份验证方法策略短信用户[登录](/azure/active-directory/authentication/concept-authentication-methods)。</span><span class="sxs-lookup"><span data-stu-id="cc603-109">The user must be enabled for SMS sign-in in the [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc603-110">权限</span><span class="sxs-lookup"><span data-stu-id="cc603-110">Permissions</span></span>

<span data-ttu-id="cc603-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc603-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="cc603-113">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="cc603-113">Permissions acting on self</span></span>

|<span data-ttu-id="cc603-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc603-114">Permission type</span></span>      | <span data-ttu-id="cc603-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cc603-115">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="cc603-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc603-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc603-117">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc603-117">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="cc603-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc603-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc603-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc603-119">Not supported.</span></span> |
| <span data-ttu-id="cc603-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc603-120">Application</span></span>                            | <span data-ttu-id="cc603-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc603-121">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="cc603-122">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="cc603-122">Permissions acting on other users</span></span>

|<span data-ttu-id="cc603-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc603-123">Permission type</span></span>      | <span data-ttu-id="cc603-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cc603-124">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="cc603-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc603-125">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc603-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc603-126">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="cc603-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc603-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc603-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc603-128">Not supported.</span></span> |
| <span data-ttu-id="cc603-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc603-129">Application</span></span>                            | <span data-ttu-id="cc603-130">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc603-130">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="cc603-131">对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="cc603-131">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="cc603-132">全局管理员</span><span class="sxs-lookup"><span data-stu-id="cc603-132">Global admin</span></span>
* <span data-ttu-id="cc603-133">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="cc603-133">Privileged authentication admin</span></span>
* <span data-ttu-id="cc603-134">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="cc603-134">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="cc603-135">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc603-135">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/enableSmsSignIn
POST /users/{id | userPrincipalName}/authentication/phoneMethods/{id}/enableSmsSignIn
```
<span data-ttu-id="cc603-136">`id`phoneType 的 `mobile` 值为 `3179e48a-750b-4051-897c-87b9720928f7` 。</span><span class="sxs-lookup"><span data-stu-id="cc603-136">The value of `id` for the `mobile` phoneType is `3179e48a-750b-4051-897c-87b9720928f7`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc603-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc603-137">Request headers</span></span>

| <span data-ttu-id="cc603-138">名称</span><span class="sxs-lookup"><span data-stu-id="cc603-138">Name</span></span>          | <span data-ttu-id="cc603-139">说明</span><span class="sxs-lookup"><span data-stu-id="cc603-139">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cc603-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc603-140">Authorization</span></span> | <span data-ttu-id="cc603-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cc603-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc603-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc603-143">Request body</span></span>

<span data-ttu-id="cc603-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cc603-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc603-145">响应</span><span class="sxs-lookup"><span data-stu-id="cc603-145">Response</span></span>

<span data-ttu-id="cc603-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cc603-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc603-148">示例</span><span class="sxs-lookup"><span data-stu-id="cc603-148">Examples</span></span>

<span data-ttu-id="cc603-149">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="cc603-149">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="cc603-150">请求</span><span class="sxs-lookup"><span data-stu-id="cc603-150">Request</span></span>

<span data-ttu-id="cc603-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cc603-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cc603-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc603-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_enablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/enableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="cc603-153">C#</span><span class="sxs-lookup"><span data-stu-id="cc603-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-enablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc603-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc603-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-enablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc603-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc603-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-enablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc603-156">Java</span><span class="sxs-lookup"><span data-stu-id="cc603-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/phoneauthenticationmethod-enablesmssignin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cc603-157">响应</span><span class="sxs-lookup"><span data-stu-id="cc603-157">Response</span></span>

<span data-ttu-id="cc603-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cc603-158">The following is an example of the response.</span></span>
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
  "description": "phoneAuthenticationMethod: enableSmsSignIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
