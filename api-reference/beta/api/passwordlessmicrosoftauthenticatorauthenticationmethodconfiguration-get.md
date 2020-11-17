---
title: 获取 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: 读取 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e47045c6eb34c393cffb89d004fb1c7a27efc49d
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086758"
---
# <a name="get-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="d2608-103">获取 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="d2608-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="d2608-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2608-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2608-105">检索 [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) 对象的属性和关系，该对象代表 Azure AD 租户的 Microsoft 身份验证器 Passwordless 电话登录 [身份验证方法策略](../resources/authenticationmethodspolicies-overview.md) 。</span><span class="sxs-lookup"><span data-stu-id="d2608-105">Retrieve the properties and relationships of the [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator Passwordless Phone Sign-in [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure AD tenant.</span></span>

> [!NOTE]
> <span data-ttu-id="d2608-106">在 Api 位于 Mirosoft Graph beta 过程中时，规划用于管理 Microsoft 身份验证器应用程序的 Api 的大量架构更改。</span><span class="sxs-lookup"><span data-stu-id="d2608-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="d2608-107">由于调用模式将发生更改，因此我们建议您不要对这些 Api 进行生产依赖。</span><span class="sxs-lookup"><span data-stu-id="d2608-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2608-108">权限</span><span class="sxs-lookup"><span data-stu-id="d2608-108">Permissions</span></span>
<span data-ttu-id="d2608-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2608-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2608-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2608-111">Permission type</span></span>|<span data-ttu-id="d2608-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d2608-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2608-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2608-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2608-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d2608-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="d2608-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2608-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2608-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2608-116">Not supported.</span></span>|
|<span data-ttu-id="d2608-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2608-117">Application</span></span>|<span data-ttu-id="d2608-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2608-118">Not supported.</span></span>|

<span data-ttu-id="d2608-119">对于委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="d2608-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="d2608-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="d2608-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="d2608-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2608-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="d2608-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2608-122">Request headers</span></span>
|<span data-ttu-id="d2608-123">名称</span><span class="sxs-lookup"><span data-stu-id="d2608-123">Name</span></span>|<span data-ttu-id="d2608-124">说明</span><span class="sxs-lookup"><span data-stu-id="d2608-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d2608-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2608-125">Authorization</span></span>|<span data-ttu-id="d2608-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d2608-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2608-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2608-128">Request body</span></span>
<span data-ttu-id="d2608-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d2608-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2608-130">响应</span><span class="sxs-lookup"><span data-stu-id="d2608-130">Response</span></span>

<span data-ttu-id="d2608-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2608-131">If successful, this method returns a `200 OK` response code and a [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2608-132">示例</span><span class="sxs-lookup"><span data-stu-id="d2608-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d2608-133">请求</span><span class="sxs-lookup"><span data-stu-id="d2608-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="d2608-134">响应</span><span class="sxs-lookup"><span data-stu-id="d2608-134">Response</span></span>
<span data-ttu-id="d2608-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d2608-135">The following is an example of the response.</span></span>

<span data-ttu-id="d2608-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d2608-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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

