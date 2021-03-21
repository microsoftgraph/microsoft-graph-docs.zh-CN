---
title: 删除 fido2AuthenticationMethodConfiguration
description: 删除 fido2AuthenticationMethodConfiguration 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1dbf6514a7dc21cb078f369d5e1e1db66f374661
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964697"
---
# <a name="delete-fido2authenticationmethodconfiguration"></a><span data-ttu-id="defde-103">删除 fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="defde-103">Delete fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="defde-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="defde-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="defde-105">将 FIDO2 身份验证方法策略还原为默认配置，以删除对 [FIDO2](../resources/fido2authenticationmethodconfiguration.md) 身份验证方法策略所做的更改。</span><span class="sxs-lookup"><span data-stu-id="defde-105">Remove changes made to the [FIDO2 authentication method policy](../resources/fido2authenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="defde-106">权限</span><span class="sxs-lookup"><span data-stu-id="defde-106">Permissions</span></span>
<span data-ttu-id="defde-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="defde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="defde-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="defde-109">Permission type</span></span>|<span data-ttu-id="defde-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="defde-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="defde-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="defde-111">Delegated (work or school account)</span></span>|<span data-ttu-id="defde-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="defde-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="defde-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="defde-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="defde-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="defde-114">Not supported.</span></span>|
|<span data-ttu-id="defde-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="defde-115">Application</span></span>|<span data-ttu-id="defde-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="defde-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="defde-117">对于委派方案，管理员需要全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="defde-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="defde-118">有关详细信息，请参阅 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="defde-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>


## <a name="http-request"></a><span data-ttu-id="defde-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="defde-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="defde-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="defde-120">Request headers</span></span>
|<span data-ttu-id="defde-121">名称</span><span class="sxs-lookup"><span data-stu-id="defde-121">Name</span></span>|<span data-ttu-id="defde-122">说明</span><span class="sxs-lookup"><span data-stu-id="defde-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="defde-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="defde-123">Authorization</span></span>|<span data-ttu-id="defde-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="defde-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="defde-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="defde-126">Request body</span></span>
<span data-ttu-id="defde-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="defde-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="defde-128">响应</span><span class="sxs-lookup"><span data-stu-id="defde-128">Response</span></span>

<span data-ttu-id="defde-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="defde-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="defde-130">示例</span><span class="sxs-lookup"><span data-stu-id="defde-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="defde-131">请求</span><span class="sxs-lookup"><span data-stu-id="defde-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


### <a name="response"></a><span data-ttu-id="defde-132">响应</span><span class="sxs-lookup"><span data-stu-id="defde-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

