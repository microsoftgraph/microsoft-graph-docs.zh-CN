---
title: 删除 userflowidentityproviders
description: 从 b2cIdentityUserFlow 中删除 identityProvider。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 4ad44addce58e8f18c0b6d582f0fd6f821cfc1c5
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401075"
---
# <a name="delete-a-userflowidentityproviders"></a><span data-ttu-id="295be-103">删除 userflowidentityproviders</span><span class="sxs-lookup"><span data-stu-id="295be-103">Delete a userflowidentityproviders</span></span>

<span data-ttu-id="295be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="295be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="295be-105">从 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象中删除标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="295be-105">Delete an identity provider from a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span> <span data-ttu-id="295be-106">有关可用于用户流的标识提供程序详细信息，请参阅 [identityProviders](../resources/identityproviderbase.md) API 参考。</span><span class="sxs-lookup"><span data-stu-id="295be-106">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityproviderbase.md) API reference.</span></span>

## <a name="permissions"></a><span data-ttu-id="295be-107">权限</span><span class="sxs-lookup"><span data-stu-id="295be-107">Permissions</span></span>

<span data-ttu-id="295be-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="295be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="295be-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="295be-110">Permission type</span></span>      | <span data-ttu-id="295be-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="295be-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="295be-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="295be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="295be-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="295be-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="295be-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="295be-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="295be-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="295be-115">Not supported.</span></span>|
|<span data-ttu-id="295be-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="295be-116">Application</span></span>| <span data-ttu-id="295be-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="295be-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="295be-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="295be-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="295be-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="295be-119">Global administrator</span></span>
* <span data-ttu-id="295be-120">外部 ID 用户流管理员</span><span class="sxs-lookup"><span data-stu-id="295be-120">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="295be-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="295be-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2cUserFlows/{userflow-id}/userflowIdentityProviders/{identityProvider-id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="295be-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="295be-122">Request headers</span></span>

|<span data-ttu-id="295be-123">名称</span><span class="sxs-lookup"><span data-stu-id="295be-123">Name</span></span>|<span data-ttu-id="295be-124">说明</span><span class="sxs-lookup"><span data-stu-id="295be-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="295be-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="295be-125">Authorization</span></span>|<span data-ttu-id="295be-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="295be-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="295be-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="295be-128">Request body</span></span>

<span data-ttu-id="295be-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="295be-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="295be-130">响应</span><span class="sxs-lookup"><span data-stu-id="295be-130">Response</span></span>

<span data-ttu-id="295be-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="295be-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="295be-132">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="295be-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="295be-133">示例</span><span class="sxs-lookup"><span data-stu-id="295be-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="295be-134">请求</span><span class="sxs-lookup"><span data-stu-id="295be-134">Request</span></span>

<span data-ttu-id="295be-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="295be-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_userflowIdentityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders/MSA-OIDC/$ref
```

### <a name="response"></a><span data-ttu-id="295be-136">响应</span><span class="sxs-lookup"><span data-stu-id="295be-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
