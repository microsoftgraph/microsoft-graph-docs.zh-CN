---
title: 删除 temporaryAccessPassAuthenticationMethodConfiguration
description: 删除对 temporaryAccessPassAuthenticationMethodConfiguration 对象所做的更改。
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 37ea21542aa9ceace151428fcf951c0a87ecbf82
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272611"
---
# <a name="delete-temporaryaccesspassauthenticationmethodconfiguration"></a><span data-ttu-id="47c92-103">删除 temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="47c92-103">Delete temporaryAccessPassAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="47c92-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47c92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47c92-105">将策略还原为默认配置，删除 [对 temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) 对象所做的更改。</span><span class="sxs-lookup"><span data-stu-id="47c92-105">Remove changes made to the [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="47c92-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="47c92-106">Permissions</span></span>
<span data-ttu-id="47c92-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47c92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47c92-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="47c92-109">Permission type</span></span>|<span data-ttu-id="47c92-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="47c92-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47c92-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47c92-111">Delegated (work or school account)</span></span>|<span data-ttu-id="47c92-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="47c92-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="47c92-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47c92-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47c92-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="47c92-114">Not supported.</span></span>|
|<span data-ttu-id="47c92-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="47c92-115">Application</span></span>|<span data-ttu-id="47c92-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="47c92-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

 <span data-ttu-id="47c92-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="47c92-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="47c92-118">有关详细信息，请参阅 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="47c92-118">For more information, see [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="47c92-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47c92-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```


## <a name="request-headers"></a><span data-ttu-id="47c92-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="47c92-120">Request headers</span></span>
|<span data-ttu-id="47c92-121">名称</span><span class="sxs-lookup"><span data-stu-id="47c92-121">Name</span></span>|<span data-ttu-id="47c92-122">说明</span><span class="sxs-lookup"><span data-stu-id="47c92-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="47c92-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="47c92-123">Authorization</span></span>|<span data-ttu-id="47c92-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="47c92-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47c92-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="47c92-126">Request body</span></span>
<span data-ttu-id="47c92-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="47c92-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47c92-128">响应</span><span class="sxs-lookup"><span data-stu-id="47c92-128">Response</span></span>

<span data-ttu-id="47c92-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="47c92-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="47c92-130">示例</span><span class="sxs-lookup"><span data-stu-id="47c92-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47c92-131">请求</span><span class="sxs-lookup"><span data-stu-id="47c92-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```


### <a name="response"></a><span data-ttu-id="47c92-132">响应</span><span class="sxs-lookup"><span data-stu-id="47c92-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
