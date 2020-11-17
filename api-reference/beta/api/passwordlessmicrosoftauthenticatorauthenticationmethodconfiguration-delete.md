---
title: 删除 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: 删除 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: eafbb6940a3d70e7191c18369e2764c137f0d674
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086640"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="77773-103">删除 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="77773-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="77773-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77773-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77773-105">通过将策略还原为其默认配置，删除对 [Microsoft 身份验证器电话登录身份验证方法策略](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) 所做的更改。</span><span class="sxs-lookup"><span data-stu-id="77773-105">Remove changes made to the [Microsoft Authenticator Phone Sign-in authentication method policy](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

> [!NOTE]
> <span data-ttu-id="77773-106">在 Api 位于 Mirosoft Graph beta 过程中时，规划用于管理 Microsoft 身份验证器应用程序的 Api 的大量架构更改。</span><span class="sxs-lookup"><span data-stu-id="77773-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="77773-107">由于调用模式将发生更改，因此我们建议您不要对这些 Api 进行生产依赖。</span><span class="sxs-lookup"><span data-stu-id="77773-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="77773-108">权限</span><span class="sxs-lookup"><span data-stu-id="77773-108">Permissions</span></span>
<span data-ttu-id="77773-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77773-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77773-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="77773-111">Permission type</span></span>|<span data-ttu-id="77773-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="77773-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77773-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77773-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77773-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="77773-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="77773-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77773-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77773-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="77773-116">Not supported.</span></span>|
|<span data-ttu-id="77773-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="77773-117">Application</span></span>|<span data-ttu-id="77773-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="77773-118">Not supported.</span></span>|

<span data-ttu-id="77773-119">对于委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：</span><span class="sxs-lookup"><span data-stu-id="77773-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="77773-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="77773-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="77773-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77773-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="77773-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="77773-122">Request headers</span></span>
|<span data-ttu-id="77773-123">名称</span><span class="sxs-lookup"><span data-stu-id="77773-123">Name</span></span>|<span data-ttu-id="77773-124">说明</span><span class="sxs-lookup"><span data-stu-id="77773-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="77773-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="77773-125">Authorization</span></span>|<span data-ttu-id="77773-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="77773-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="77773-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="77773-128">Request body</span></span>
<span data-ttu-id="77773-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="77773-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77773-130">响应</span><span class="sxs-lookup"><span data-stu-id="77773-130">Response</span></span>

<span data-ttu-id="77773-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="77773-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="77773-132">示例</span><span class="sxs-lookup"><span data-stu-id="77773-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="77773-133">请求</span><span class="sxs-lookup"><span data-stu-id="77773-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="77773-134">响应</span><span class="sxs-lookup"><span data-stu-id="77773-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

