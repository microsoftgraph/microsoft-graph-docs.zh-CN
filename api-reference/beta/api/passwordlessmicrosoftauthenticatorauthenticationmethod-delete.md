---
title: 删除 passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: 删除无密码MicrosoftAuthenticatorAuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5bd76dcb0652fdea395592ff916cd37eac789384
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515959"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethod-deprecated"></a><span data-ttu-id="e18c8-103">删除已弃 (passwordlessMicrosoftAuthenticatorAuthenticationMethod) </span><span class="sxs-lookup"><span data-stu-id="e18c8-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethod (deprecated)</span></span>
<span data-ttu-id="e18c8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e18c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e18c8-105">删除用户的 [Microsoft Authenticator Passwordless Phone Sign-in 方法](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e18c8-105">Deletes a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!CAUTION]
> <span data-ttu-id="e18c8-106">Microsoft Authenticator 无密码电话登录方法 API 已弃用，将于 2020 年 12 月 31 日停止返回结果。</span><span class="sxs-lookup"><span data-stu-id="e18c8-106">The Microsoft Authenticator Passwordless Phone Sign-in method API is deprecated and will stop returning results on December 31, 2020.</span></span> <span data-ttu-id="e18c8-107">请使用新的 [Microsoft Authenticator 身份验证方法](../resources/microsoftAuthenticatorAuthenticationMethod.md)。</span><span class="sxs-lookup"><span data-stu-id="e18c8-107">Please use the new [Microsoft Authenticator Authentication Method](../resources/microsoftAuthenticatorAuthenticationMethod.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e18c8-108">权限</span><span class="sxs-lookup"><span data-stu-id="e18c8-108">Permissions</span></span>

<span data-ttu-id="e18c8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e18c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="e18c8-111">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="e18c8-111">Permissions acting on self</span></span>

|<span data-ttu-id="e18c8-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e18c8-112">Permission type</span></span>      | <span data-ttu-id="e18c8-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e18c8-113">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="e18c8-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e18c8-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="e18c8-115">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e18c8-115">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="e18c8-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e18c8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e18c8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e18c8-117">Not supported.</span></span> |
| <span data-ttu-id="e18c8-118">Application</span><span class="sxs-lookup"><span data-stu-id="e18c8-118">Application</span></span>                            | <span data-ttu-id="e18c8-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="e18c8-119">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="e18c8-120">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="e18c8-120">Permissions acting on other users</span></span>

|<span data-ttu-id="e18c8-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="e18c8-121">Permission type</span></span>      | <span data-ttu-id="e18c8-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e18c8-122">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="e18c8-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e18c8-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="e18c8-124">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e18c8-124">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="e18c8-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e18c8-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e18c8-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="e18c8-126">Not supported.</span></span> |
| <span data-ttu-id="e18c8-127">Application</span><span class="sxs-lookup"><span data-stu-id="e18c8-127">Application</span></span>                            | <span data-ttu-id="e18c8-128">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e18c8-128">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="e18c8-129">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="e18c8-129">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="e18c8-130">全局管理员</span><span class="sxs-lookup"><span data-stu-id="e18c8-130">Global admin</span></span>
* <span data-ttu-id="e18c8-131">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="e18c8-131">Privileged authentication admin</span></span>
* <span data-ttu-id="e18c8-132">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="e18c8-132">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="e18c8-133">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e18c8-133">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e18c8-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="e18c8-134">Request headers</span></span>
|<span data-ttu-id="e18c8-135">名称</span><span class="sxs-lookup"><span data-stu-id="e18c8-135">Name</span></span>|<span data-ttu-id="e18c8-136">说明</span><span class="sxs-lookup"><span data-stu-id="e18c8-136">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e18c8-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="e18c8-137">Authorization</span></span>|<span data-ttu-id="e18c8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e18c8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e18c8-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="e18c8-140">Request body</span></span>
<span data-ttu-id="e18c8-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e18c8-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e18c8-142">响应</span><span class="sxs-lookup"><span data-stu-id="e18c8-142">Response</span></span>

<span data-ttu-id="e18c8-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e18c8-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e18c8-145">示例</span><span class="sxs-lookup"><span data-stu-id="e18c8-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e18c8-146">请求</span><span class="sxs-lookup"><span data-stu-id="e18c8-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e18c8-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="e18c8-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```
# <a name="c"></a>[<span data-ttu-id="e18c8-148">C#</span><span class="sxs-lookup"><span data-stu-id="e18c8-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e18c8-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e18c8-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e18c8-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e18c8-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e18c8-151">Java</span><span class="sxs-lookup"><span data-stu-id="e18c8-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e18c8-152">响应</span><span class="sxs-lookup"><span data-stu-id="e18c8-152">Response</span></span>
<span data-ttu-id="e18c8-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e18c8-153">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

