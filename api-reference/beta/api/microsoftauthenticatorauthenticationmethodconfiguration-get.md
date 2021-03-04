---
title: 获取 microsoftAuthenticatorAuthenticationMethodConfiguration
description: 读取 microsoftAuthenticatorAuthenticationMethodConfiguration 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 32470fb4ebce664fadce95982adb0d2d61bf6f03
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443690"
---
# <a name="get-microsoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="f3075-103">获取 microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="f3075-103">Get microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="f3075-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3075-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3075-105">检索 [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) 对象的属性和关系，该对象代表 Azure AD 租户的 Microsoft Authenticator 身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="f3075-105">Retrieve the properties and relationships of the [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3075-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f3075-106">Permissions</span></span>
<span data-ttu-id="f3075-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f3075-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3075-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f3075-109">Permission type</span></span>|<span data-ttu-id="f3075-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f3075-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3075-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f3075-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f3075-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f3075-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="f3075-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f3075-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3075-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3075-114">Not supported.</span></span>|
|<span data-ttu-id="f3075-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f3075-115">Application</span></span>|<span data-ttu-id="f3075-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f3075-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="f3075-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="f3075-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="f3075-118">有关详细信息，请参阅 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="f3075-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="f3075-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f3075-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="f3075-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f3075-120">Request headers</span></span>
|<span data-ttu-id="f3075-121">名称</span><span class="sxs-lookup"><span data-stu-id="f3075-121">Name</span></span>|<span data-ttu-id="f3075-122">说明</span><span class="sxs-lookup"><span data-stu-id="f3075-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f3075-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3075-123">Authorization</span></span>|<span data-ttu-id="f3075-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f3075-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3075-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f3075-126">Request body</span></span>
<span data-ttu-id="f3075-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f3075-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3075-128">响应</span><span class="sxs-lookup"><span data-stu-id="f3075-128">Response</span></span>

<span data-ttu-id="f3075-129">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f3075-129">If successful, this method returns a `200 OK` response code and a [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f3075-130">示例</span><span class="sxs-lookup"><span data-stu-id="f3075-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f3075-131">请求</span><span class="sxs-lookup"><span data-stu-id="f3075-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="f3075-132">响应</span><span class="sxs-lookup"><span data-stu-id="f3075-132">Response</span></span>
<span data-ttu-id="f3075-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f3075-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
    "id": "129ae788-e788-129a-88e7-9a1288e79a12",
    "state": "String"
  }
}
```

