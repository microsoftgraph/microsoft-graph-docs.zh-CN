---
title: 获取 passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: 读取无密码MicrosoftAuthenticatorAuthenticationMethod 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 56d5e5223480f09bb9d2626a48938a783fbaa2bc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447778"
---
# <a name="get-passwordlessmicrosoftauthenticatorauthenticationmethod-deprecated"></a><span data-ttu-id="8b02b-103">获取 passwordlessMicrosoftAuthenticatorAuthenticationMethod (已弃) </span><span class="sxs-lookup"><span data-stu-id="8b02b-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethod (deprecated)</span></span>
<span data-ttu-id="8b02b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b02b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b02b-105">检索用户的单个 Microsoft [Authenticator Passwordless Phone Sign-in 方法](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8b02b-105">Retrieve a user's single [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!CAUTION]
> <span data-ttu-id="8b02b-106">Microsoft Authenticator 无密码电话登录方法 API 已弃用，将于 2020 年 12 月 31 日停止返回结果。</span><span class="sxs-lookup"><span data-stu-id="8b02b-106">The Microsoft Authenticator Passwordless Phone Sign-in method API is deprecated and will stop returning results on December 31, 2020.</span></span> <span data-ttu-id="8b02b-107">请使用新的 [Microsoft Authenticator 身份验证方法](../resources/microsoftAuthenticatorAuthenticationMethod.md)。</span><span class="sxs-lookup"><span data-stu-id="8b02b-107">Please use the new [Microsoft Authenticator Authentication Method](../resources/microsoftAuthenticatorAuthenticationMethod.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8b02b-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="8b02b-108">Permissions</span></span>

<span data-ttu-id="8b02b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b02b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="8b02b-111">自行操作的权限</span><span class="sxs-lookup"><span data-stu-id="8b02b-111">Permissions acting on self</span></span>

|<span data-ttu-id="8b02b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b02b-112">Permission type</span></span>      | <span data-ttu-id="8b02b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8b02b-113">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="8b02b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b02b-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b02b-115">UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b02b-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="8b02b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b02b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b02b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b02b-117">Not supported.</span></span> |
| <span data-ttu-id="8b02b-118">Application</span><span class="sxs-lookup"><span data-stu-id="8b02b-118">Application</span></span>                            | <span data-ttu-id="8b02b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b02b-119">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="8b02b-120">对其他用户操作的权限</span><span class="sxs-lookup"><span data-stu-id="8b02b-120">Permissions acting on other users</span></span>

|<span data-ttu-id="8b02b-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b02b-121">Permission type</span></span>      | <span data-ttu-id="8b02b-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8b02b-122">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="8b02b-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b02b-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b02b-124">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b02b-124">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="8b02b-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b02b-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b02b-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b02b-126">Not supported.</span></span> |
| <span data-ttu-id="8b02b-127">Application</span><span class="sxs-lookup"><span data-stu-id="8b02b-127">Application</span></span>                            | <span data-ttu-id="8b02b-128">UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b02b-128">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="8b02b-129">对于管理员正在操作其他用户的委派方案，管理员需要以下 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="8b02b-129">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="8b02b-130">全局管理员</span><span class="sxs-lookup"><span data-stu-id="8b02b-130">Global admin</span></span>
* <span data-ttu-id="8b02b-131">全局读取者</span><span class="sxs-lookup"><span data-stu-id="8b02b-131">Global reader</span></span>
* <span data-ttu-id="8b02b-132">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="8b02b-132">Privileged authentication admin</span></span>
* <span data-ttu-id="8b02b-133">身份验证管理员 (只能看到屏蔽的电话号码) </span><span class="sxs-lookup"><span data-stu-id="8b02b-133">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="8b02b-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b02b-134">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8b02b-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b02b-135">Request headers</span></span>
|<span data-ttu-id="8b02b-136">名称</span><span class="sxs-lookup"><span data-stu-id="8b02b-136">Name</span></span>|<span data-ttu-id="8b02b-137">说明</span><span class="sxs-lookup"><span data-stu-id="8b02b-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8b02b-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b02b-138">Authorization</span></span>|<span data-ttu-id="8b02b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8b02b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b02b-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b02b-141">Request body</span></span>
<span data-ttu-id="8b02b-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8b02b-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b02b-143">响应</span><span class="sxs-lookup"><span data-stu-id="8b02b-143">Response</span></span>

<span data-ttu-id="8b02b-144">如果成功，此方法在响应正文中返回响应代码和请求的 `200 OK` [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8b02b-144">If successful, this method returns a `200 OK` response code and the requested [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b02b-145">示例</span><span class="sxs-lookup"><span data-stu-id="8b02b-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8b02b-146">请求</span><span class="sxs-lookup"><span data-stu-id="8b02b-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8b02b-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b02b-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```
# <a name="c"></a>[<span data-ttu-id="8b02b-148">C#</span><span class="sxs-lookup"><span data-stu-id="8b02b-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b02b-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b02b-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b02b-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b02b-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b02b-151">Java</span><span class="sxs-lookup"><span data-stu-id="8b02b-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordlessmicrosoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8b02b-152">响应</span><span class="sxs-lookup"><span data-stu-id="8b02b-152">Response</span></span>
<span data-ttu-id="8b02b-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8b02b-153">The following is an example of the response.</span></span>

<span data-ttu-id="8b02b-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8b02b-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": {
      "id": "R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1",
      "displayName": "My mobile phone",
      "creationDateTime": "2020-09-02T04:16:49Z"
  }
}
```

