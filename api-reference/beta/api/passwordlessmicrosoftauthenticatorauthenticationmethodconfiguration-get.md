---
title: 获取 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: 读取无密码MicrosoftAuthenticatorAuthenticationMethodConfiguration 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c21d1c8601715beef6f056defbf203afa417ac0c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447757"
---
# <a name="get-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-deprecated"></a><span data-ttu-id="1e633-103">获取 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (弃) </span><span class="sxs-lookup"><span data-stu-id="1e633-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (deprecated)</span></span>
<span data-ttu-id="1e633-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e633-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e633-105">检索无[密码MicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)对象的属性和关系，该对象代表 Azure AD 租户的 Microsoft Authenticator Passwordless Phone 登录身份验证方法策略。 [](../resources/authenticationmethodspolicies-overview.md)</span><span class="sxs-lookup"><span data-stu-id="1e633-105">Retrieve the properties and relationships of the [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator Passwordless Phone Sign-in [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure AD tenant.</span></span>

> [!CAUTION]
> <span data-ttu-id="1e633-106">Microsoft Authenticator 无密码电话登录身份验证方法策略 API 已弃用，并停止在 2020 年 12 月 31 日返回结果。</span><span class="sxs-lookup"><span data-stu-id="1e633-106">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="1e633-107">请使用新的 [Microsoft Authenticator 身份验证方法策略](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="1e633-107">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1e633-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="1e633-108">Permissions</span></span>
<span data-ttu-id="1e633-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e633-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e633-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e633-111">Permission type</span></span>|<span data-ttu-id="1e633-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e633-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e633-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e633-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e633-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1e633-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="1e633-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e633-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e633-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e633-116">Not supported.</span></span>|
|<span data-ttu-id="1e633-117">Application</span><span class="sxs-lookup"><span data-stu-id="1e633-117">Application</span></span>|<span data-ttu-id="1e633-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e633-118">Not supported.</span></span>|

<span data-ttu-id="1e633-119">对于委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="1e633-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="1e633-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="1e633-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="1e633-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e633-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="1e633-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e633-122">Request headers</span></span>
|<span data-ttu-id="1e633-123">名称</span><span class="sxs-lookup"><span data-stu-id="1e633-123">Name</span></span>|<span data-ttu-id="1e633-124">说明</span><span class="sxs-lookup"><span data-stu-id="1e633-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1e633-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e633-125">Authorization</span></span>|<span data-ttu-id="1e633-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1e633-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e633-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e633-128">Request body</span></span>
<span data-ttu-id="1e633-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1e633-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e633-130">响应</span><span class="sxs-lookup"><span data-stu-id="1e633-130">Response</span></span>

<span data-ttu-id="1e633-131">如果成功，此方法在响应正文中返回响应代码和无密码 `200 OK` [MicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1e633-131">If successful, this method returns a `200 OK` response code and a [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1e633-132">示例</span><span class="sxs-lookup"><span data-stu-id="1e633-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1e633-133">请求</span><span class="sxs-lookup"><span data-stu-id="1e633-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="1e633-134">响应</span><span class="sxs-lookup"><span data-stu-id="1e633-134">Response</span></span>
<span data-ttu-id="1e633-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1e633-135">The following is an example of the response.</span></span>

<span data-ttu-id="1e633-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1e633-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
    "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
    "id": "PasswordlessMicrosoftAuthenticator",
    "state": "enabled",
    "includeTargets": [
        {
            "targetType": "group",
            "id": "all_users",
            "isRegistrationRequired": false,
            "useForSignIn": true
        }
    ]
}
```

