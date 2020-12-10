---
title: 删除 emailAuthenticationMethodConfiguration
description: 删除一个 emailAuthenticationMethodConfiguration 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d5b9ac408a9de38ceb75f8ee04ee3c442705936d
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617111"
---
# <a name="delete-emailauthenticationmethodconfiguration"></a><span data-ttu-id="b7328-103">删除 emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="b7328-103">Delete emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="b7328-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7328-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7328-105">通过将策略还原为其默认配置，删除对 [电子邮件身份验证方法策略](../resources/emailauthenticationmethodconfiguration.md) 所做的更改。</span><span class="sxs-lookup"><span data-stu-id="b7328-105">Remove changes made to the [email authentication method policy](../resources/emailauthenticationmethodconfiguration.md) by reverting the policy to its default configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7328-106">权限</span><span class="sxs-lookup"><span data-stu-id="b7328-106">Permissions</span></span>
<span data-ttu-id="b7328-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7328-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7328-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7328-109">Permission type</span></span>|<span data-ttu-id="b7328-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b7328-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7328-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7328-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b7328-112">Policy 写的 AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b7328-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="b7328-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7328-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7328-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7328-114">Not supported.</span></span>|
|<span data-ttu-id="b7328-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7328-115">Application</span></span>|<span data-ttu-id="b7328-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7328-116">Not supported.</span></span>|

<span data-ttu-id="b7328-117">对于委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="b7328-117">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="b7328-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="b7328-118">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="b7328-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7328-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
DELETE /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

## <a name="request-headers"></a><span data-ttu-id="b7328-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7328-120">Request headers</span></span>

|<span data-ttu-id="b7328-121">名称</span><span class="sxs-lookup"><span data-stu-id="b7328-121">Name</span></span>|<span data-ttu-id="b7328-122">说明</span><span class="sxs-lookup"><span data-stu-id="b7328-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b7328-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7328-123">Authorization</span></span>|<span data-ttu-id="b7328-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b7328-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7328-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7328-126">Request body</span></span>

<span data-ttu-id="b7328-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b7328-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7328-128">响应</span><span class="sxs-lookup"><span data-stu-id="b7328-128">Response</span></span>

<span data-ttu-id="b7328-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b7328-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b7328-130">示例</span><span class="sxs-lookup"><span data-stu-id="b7328-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b7328-131">请求</span><span class="sxs-lookup"><span data-stu-id="b7328-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethodconfiguration"
}
-->

```http
DELETE https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

### <a name="response"></a><span data-ttu-id="b7328-132">响应</span><span class="sxs-lookup"><span data-stu-id="b7328-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```

