---
title: 删除 microsoftAuthenticatorAuthenticationMethodConfiguration
description: 删除 microsoftAuthenticatorAuthenticationMethodConfiguration 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 93a16ae2865fcdb85963c7e8aded8e5ca6727720
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202739"
---
# <a name="delete-microsoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="6f09f-103">删除 microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="6f09f-103">Delete microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="6f09f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f09f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f09f-105">将 Microsoft Authenticator 身份验证方法策略还原为默认配置，以删除对 Microsoft [Authenticator](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) 身份验证方法策略所做的更改。</span><span class="sxs-lookup"><span data-stu-id="6f09f-105">Remove changes made to the [Microsoft Authenticator authentication method policy](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f09f-106">权限</span><span class="sxs-lookup"><span data-stu-id="6f09f-106">Permissions</span></span>
<span data-ttu-id="6f09f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6f09f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f09f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f09f-109">Permission type</span></span>|<span data-ttu-id="6f09f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6f09f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f09f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f09f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6f09f-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6f09f-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="6f09f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f09f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f09f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f09f-114">Not supported.</span></span>|
|<span data-ttu-id="6f09f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f09f-115">Application</span></span>|<span data-ttu-id="6f09f-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6f09f-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="6f09f-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="6f09f-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="6f09f-118">有关详细信息，请参阅 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="6f09f-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="6f09f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f09f-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="6f09f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f09f-120">Request headers</span></span>
|<span data-ttu-id="6f09f-121">名称</span><span class="sxs-lookup"><span data-stu-id="6f09f-121">Name</span></span>|<span data-ttu-id="6f09f-122">说明</span><span class="sxs-lookup"><span data-stu-id="6f09f-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6f09f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f09f-123">Authorization</span></span>|<span data-ttu-id="6f09f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6f09f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f09f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f09f-126">Request body</span></span>
<span data-ttu-id="6f09f-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6f09f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f09f-128">响应</span><span class="sxs-lookup"><span data-stu-id="6f09f-128">Response</span></span>

<span data-ttu-id="6f09f-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6f09f-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6f09f-130">示例</span><span class="sxs-lookup"><span data-stu-id="6f09f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6f09f-131">请求</span><span class="sxs-lookup"><span data-stu-id="6f09f-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6f09f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f09f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```
# <a name="c"></a>[<span data-ttu-id="6f09f-133">C#</span><span class="sxs-lookup"><span data-stu-id="6f09f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-microsoftauthenticatorauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f09f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f09f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-microsoftauthenticatorauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f09f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f09f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-microsoftauthenticatorauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f09f-136">Java</span><span class="sxs-lookup"><span data-stu-id="6f09f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-microsoftauthenticatorauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6f09f-137">响应</span><span class="sxs-lookup"><span data-stu-id="6f09f-137">Response</span></span>
<span data-ttu-id="6f09f-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6f09f-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

