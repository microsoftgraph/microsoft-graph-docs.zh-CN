---
title: 删除 fido2AuthenticationMethodConfiguration
description: 删除 fido2AuthenticationMethodConfiguration 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8dbb2b7d2c8948763ffc48ac299cc3f2f330498a
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418195"
---
# <a name="delete-fido2authenticationmethodconfiguration"></a><span data-ttu-id="14bd1-103">删除 fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="14bd1-103">Delete fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="14bd1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14bd1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14bd1-105">通过将策略还原为其默认配置，删除对 [FIDO2 身份验证方法策略](../resources/fido2authenticationmethodconfiguration.md) 所做的更改。</span><span class="sxs-lookup"><span data-stu-id="14bd1-105">Remove changes made to the [FIDO2 authentication method policy](../resources/fido2authenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="14bd1-106">权限</span><span class="sxs-lookup"><span data-stu-id="14bd1-106">Permissions</span></span>
<span data-ttu-id="14bd1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14bd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="14bd1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="14bd1-109">Permission type</span></span>|<span data-ttu-id="14bd1-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="14bd1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14bd1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14bd1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="14bd1-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="14bd1-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="14bd1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14bd1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14bd1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="14bd1-114">Not supported.</span></span>|
|<span data-ttu-id="14bd1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="14bd1-115">Application</span></span>|<span data-ttu-id="14bd1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="14bd1-116">Not supported.</span></span>|

<span data-ttu-id="14bd1-117">对于委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="14bd1-117">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="14bd1-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="14bd1-118">Global admin</span></span>
* <span data-ttu-id="14bd1-119">全局读取者</span><span class="sxs-lookup"><span data-stu-id="14bd1-119">Global reader</span></span>
* <span data-ttu-id="14bd1-120">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="14bd1-120">Privileged authentication admin</span></span>
* <span data-ttu-id="14bd1-121">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="14bd1-121">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="14bd1-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14bd1-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="14bd1-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="14bd1-123">Request headers</span></span>
|<span data-ttu-id="14bd1-124">名称</span><span class="sxs-lookup"><span data-stu-id="14bd1-124">Name</span></span>|<span data-ttu-id="14bd1-125">说明</span><span class="sxs-lookup"><span data-stu-id="14bd1-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="14bd1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="14bd1-126">Authorization</span></span>|<span data-ttu-id="14bd1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14bd1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="14bd1-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="14bd1-129">Request body</span></span>
<span data-ttu-id="14bd1-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="14bd1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14bd1-131">响应</span><span class="sxs-lookup"><span data-stu-id="14bd1-131">Response</span></span>

<span data-ttu-id="14bd1-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="14bd1-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="14bd1-133">示例</span><span class="sxs-lookup"><span data-stu-id="14bd1-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="14bd1-134">请求</span><span class="sxs-lookup"><span data-stu-id="14bd1-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethodconfiguration"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```


### <a name="response"></a><span data-ttu-id="14bd1-135">响应</span><span class="sxs-lookup"><span data-stu-id="14bd1-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

