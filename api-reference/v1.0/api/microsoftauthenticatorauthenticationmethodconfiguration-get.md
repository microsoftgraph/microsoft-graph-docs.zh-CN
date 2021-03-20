---
title: 获取 microsoftAuthenticatorAuthenticationMethodConfiguration
description: 读取 microsoftAuthenticatorAuthenticationMethodConfiguration 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f94c20bcfb29de6af6ec77371594b367ed93e88b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948974"
---
# <a name="get-microsoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="8f655-103">获取 microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="8f655-103">Get microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="8f655-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f655-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8f655-105">检索 [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) 对象的属性和关系，该对象表示 Azure AD 租户的 Microsoft Authenticator 身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="8f655-105">Retrieve the properties and relationships of the [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f655-106">权限</span><span class="sxs-lookup"><span data-stu-id="8f655-106">Permissions</span></span>
<span data-ttu-id="8f655-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f655-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f655-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f655-109">Permission type</span></span>|<span data-ttu-id="8f655-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f655-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f655-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f655-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8f655-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8f655-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="8f655-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f655-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f655-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f655-114">Not supported.</span></span>|
|<span data-ttu-id="8f655-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f655-115">Application</span></span>|<span data-ttu-id="8f655-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8f655-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="8f655-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="8f655-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="8f655-118">有关详细信息，请参阅 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="8f655-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="8f655-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f655-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="8f655-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f655-120">Request headers</span></span>
|<span data-ttu-id="8f655-121">名称</span><span class="sxs-lookup"><span data-stu-id="8f655-121">Name</span></span>|<span data-ttu-id="8f655-122">说明</span><span class="sxs-lookup"><span data-stu-id="8f655-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8f655-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f655-123">Authorization</span></span>|<span data-ttu-id="8f655-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f655-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f655-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f655-126">Request body</span></span>
<span data-ttu-id="8f655-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8f655-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f655-128">响应</span><span class="sxs-lookup"><span data-stu-id="8f655-128">Response</span></span>

<span data-ttu-id="8f655-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8f655-129">If successful, this method returns a `200 OK` response code and a [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f655-130">示例</span><span class="sxs-lookup"><span data-stu-id="8f655-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8f655-131">请求</span><span class="sxs-lookup"><span data-stu-id="8f655-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="8f655-132">响应</span><span class="sxs-lookup"><span data-stu-id="8f655-132">Response</span></span>
<span data-ttu-id="8f655-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8f655-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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

