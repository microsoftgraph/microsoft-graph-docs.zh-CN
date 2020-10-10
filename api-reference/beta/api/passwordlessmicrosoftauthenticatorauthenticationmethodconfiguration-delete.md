---
title: 删除 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: 删除 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3200e95acdee4042c3933d5926662d6e49d52052
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418282"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="c7501-103">删除 passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="c7501-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="c7501-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7501-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7501-105">通过将策略还原为其默认配置，删除对 [Microsoft 身份验证器电话登录身份验证方法策略](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) 所做的更改。</span><span class="sxs-lookup"><span data-stu-id="c7501-105">Remove changes made to the [Microsoft Authenticator Phone Sign-in authentication method policy](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

> [!NOTE]
> <span data-ttu-id="c7501-106">在 Api 位于 Mirosoft Graph beta 过程中时，规划用于管理 Microsoft 身份验证器应用程序的 Api 的大量架构更改。</span><span class="sxs-lookup"><span data-stu-id="c7501-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="c7501-107">由于调用模式将发生更改，因此我们建议您不要对这些 Api 进行生产依赖。</span><span class="sxs-lookup"><span data-stu-id="c7501-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7501-108">权限</span><span class="sxs-lookup"><span data-stu-id="c7501-108">Permissions</span></span>
<span data-ttu-id="c7501-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7501-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7501-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7501-111">Permission type</span></span>|<span data-ttu-id="c7501-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c7501-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7501-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7501-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7501-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c7501-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="c7501-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7501-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7501-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7501-116">Not supported.</span></span>|
|<span data-ttu-id="c7501-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7501-117">Application</span></span>|<span data-ttu-id="c7501-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7501-118">Not supported.</span></span>|

<span data-ttu-id="c7501-119">对于委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="c7501-119">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="c7501-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="c7501-120">Global admin</span></span>
* <span data-ttu-id="c7501-121">全局读取者</span><span class="sxs-lookup"><span data-stu-id="c7501-121">Global reader</span></span>
* <span data-ttu-id="c7501-122">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="c7501-122">Privileged authentication admin</span></span>
* <span data-ttu-id="c7501-123">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="c7501-123">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="c7501-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7501-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="c7501-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7501-125">Request headers</span></span>
|<span data-ttu-id="c7501-126">名称</span><span class="sxs-lookup"><span data-stu-id="c7501-126">Name</span></span>|<span data-ttu-id="c7501-127">说明</span><span class="sxs-lookup"><span data-stu-id="c7501-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c7501-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7501-128">Authorization</span></span>|<span data-ttu-id="c7501-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c7501-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7501-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7501-131">Request body</span></span>
<span data-ttu-id="c7501-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c7501-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7501-133">响应</span><span class="sxs-lookup"><span data-stu-id="c7501-133">Response</span></span>

<span data-ttu-id="c7501-134">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c7501-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c7501-135">示例</span><span class="sxs-lookup"><span data-stu-id="c7501-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7501-136">请求</span><span class="sxs-lookup"><span data-stu-id="c7501-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="c7501-137">响应</span><span class="sxs-lookup"><span data-stu-id="c7501-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

