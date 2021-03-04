---
title: 删除 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: 删除无密码MicrosoftAuthenticatorAuthenticationMethodConfiguration 对象。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7961f575265ef4fc8ddae23b9e36cd7352a0ae85
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447764"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-deprecated"></a><span data-ttu-id="99260-103">删除已弃 (passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration) </span><span class="sxs-lookup"><span data-stu-id="99260-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (deprecated)</span></span>
<span data-ttu-id="99260-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99260-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99260-105">通过将 Microsoft [Authenticator Phone 登录](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) 身份验证方法策略恢复为默认配置，删除对 Microsoft Authenticator Phone 登录身份验证方法策略所做的更改。</span><span class="sxs-lookup"><span data-stu-id="99260-105">Remove changes made to the [Microsoft Authenticator Phone Sign-in authentication method policy](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

> [!CAUTION]
> <span data-ttu-id="99260-106">Microsoft Authenticator 无密码电话登录身份验证方法策略 API 已弃用，并停止在 2020 年 12 月 31 日返回结果。</span><span class="sxs-lookup"><span data-stu-id="99260-106">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="99260-107">请使用新的 [Microsoft Authenticator 身份验证方法策略](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="99260-107">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="99260-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="99260-108">Permissions</span></span>
<span data-ttu-id="99260-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99260-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99260-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="99260-111">Permission type</span></span>|<span data-ttu-id="99260-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99260-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99260-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99260-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99260-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="99260-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="99260-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99260-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99260-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="99260-116">Not supported.</span></span>|
|<span data-ttu-id="99260-117">Application</span><span class="sxs-lookup"><span data-stu-id="99260-117">Application</span></span>|<span data-ttu-id="99260-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="99260-118">Not supported.</span></span>|

<span data-ttu-id="99260-119">对于委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="99260-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="99260-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="99260-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="99260-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99260-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="99260-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="99260-122">Request headers</span></span>
|<span data-ttu-id="99260-123">名称</span><span class="sxs-lookup"><span data-stu-id="99260-123">Name</span></span>|<span data-ttu-id="99260-124">说明</span><span class="sxs-lookup"><span data-stu-id="99260-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="99260-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="99260-125">Authorization</span></span>|<span data-ttu-id="99260-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="99260-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="99260-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="99260-128">Request body</span></span>
<span data-ttu-id="99260-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="99260-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99260-130">响应</span><span class="sxs-lookup"><span data-stu-id="99260-130">Response</span></span>

<span data-ttu-id="99260-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="99260-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="99260-132">示例</span><span class="sxs-lookup"><span data-stu-id="99260-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="99260-133">请求</span><span class="sxs-lookup"><span data-stu-id="99260-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="99260-134">响应</span><span class="sxs-lookup"><span data-stu-id="99260-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

