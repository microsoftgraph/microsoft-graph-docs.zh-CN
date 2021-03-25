---
title: 获取 microsoftAuthenticatorAuthenticationMethodConfiguration
description: 读取 microsoftAuthenticatorAuthenticationMethodConfiguration 对象的属性和关系。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ab22fdac70f4d7101a8610a5a96ca5bdfa84d943
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202867"
---
# <a name="get-microsoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="e517e-103">获取 microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="e517e-103">Get microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="e517e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e517e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e517e-105">检索 [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) 对象的属性和关系，该对象表示 Azure AD 租户的 Microsoft Authenticator 身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="e517e-105">Retrieve the properties and relationships of the [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e517e-106">权限</span><span class="sxs-lookup"><span data-stu-id="e517e-106">Permissions</span></span>
<span data-ttu-id="e517e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e517e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e517e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e517e-109">Permission type</span></span>|<span data-ttu-id="e517e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e517e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e517e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e517e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e517e-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e517e-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="e517e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e517e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e517e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e517e-114">Not supported.</span></span>|
|<span data-ttu-id="e517e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e517e-115">Application</span></span>|<span data-ttu-id="e517e-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e517e-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="e517e-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="e517e-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="e517e-118">有关详细信息，请参阅 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="e517e-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="e517e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e517e-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="e517e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e517e-120">Request headers</span></span>
|<span data-ttu-id="e517e-121">名称</span><span class="sxs-lookup"><span data-stu-id="e517e-121">Name</span></span>|<span data-ttu-id="e517e-122">说明</span><span class="sxs-lookup"><span data-stu-id="e517e-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e517e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e517e-123">Authorization</span></span>|<span data-ttu-id="e517e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e517e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e517e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e517e-126">Request body</span></span>
<span data-ttu-id="e517e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e517e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e517e-128">响应</span><span class="sxs-lookup"><span data-stu-id="e517e-128">Response</span></span>

<span data-ttu-id="e517e-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e517e-129">If successful, this method returns a `200 OK` response code and a [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e517e-130">示例</span><span class="sxs-lookup"><span data-stu-id="e517e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e517e-131">请求</span><span class="sxs-lookup"><span data-stu-id="e517e-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e517e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e517e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```
# <a name="c"></a>[<span data-ttu-id="e517e-133">C#</span><span class="sxs-lookup"><span data-stu-id="e517e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-microsoftauthenticatorauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e517e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e517e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-microsoftauthenticatorauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e517e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e517e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-microsoftauthenticatorauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e517e-136">Java</span><span class="sxs-lookup"><span data-stu-id="e517e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-microsoftauthenticatorauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e517e-137">响应</span><span class="sxs-lookup"><span data-stu-id="e517e-137">Response</span></span>
<span data-ttu-id="e517e-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e517e-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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

