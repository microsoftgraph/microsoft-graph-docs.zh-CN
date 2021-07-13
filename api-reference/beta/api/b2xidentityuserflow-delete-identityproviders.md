---
title: '从 b2xIdentityUserFlow 中删除 identityProvider (弃) '
description: '从 b2xIdentityUserFlow 中删除 identityProvider。  (已弃) '
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 94310d9c4ffa629638721fd248866ab685b8f506
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400948"
---
# <a name="delete-identityprovider-from-b2xidentityuserflow-deprecated"></a><span data-ttu-id="ccde4-104">从 b2xIdentityUserFlow 中删除 identityProvider (弃) </span><span class="sxs-lookup"><span data-stu-id="ccde4-104">Delete identityProvider from b2xIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="ccde4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccde4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="ccde4-106">从 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象中删除标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="ccde4-106">Delete an identity provider from a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span> <span data-ttu-id="ccde4-107">对于自助注册用户流，值可以是 `Google-OAUTH` 或 `Facebook-OAUTH` 。</span><span class="sxs-lookup"><span data-stu-id="ccde4-107">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccde4-108">权限</span><span class="sxs-lookup"><span data-stu-id="ccde4-108">Permissions</span></span>

<span data-ttu-id="ccde4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ccde4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccde4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ccde4-111">Permission type</span></span>      | <span data-ttu-id="ccde4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ccde4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccde4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ccde4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ccde4-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccde4-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ccde4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ccde4-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ccde4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccde4-116">Not supported.</span></span>|
|<span data-ttu-id="ccde4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ccde4-117">Application</span></span>| <span data-ttu-id="ccde4-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccde4-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="ccde4-119">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="ccde4-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ccde4-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="ccde4-120">Global administrator</span></span>
* <span data-ttu-id="ccde4-121">外部标识用户Flow管理员</span><span class="sxs-lookup"><span data-stu-id="ccde4-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ccde4-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ccde4-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2xUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ccde4-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="ccde4-123">Request headers</span></span>

|<span data-ttu-id="ccde4-124">名称</span><span class="sxs-lookup"><span data-stu-id="ccde4-124">Name</span></span>|<span data-ttu-id="ccde4-125">说明</span><span class="sxs-lookup"><span data-stu-id="ccde4-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ccde4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccde4-126">Authorization</span></span>|<span data-ttu-id="ccde4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ccde4-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccde4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="ccde4-129">Request body</span></span>

<span data-ttu-id="ccde4-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ccde4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccde4-131">响应</span><span class="sxs-lookup"><span data-stu-id="ccde4-131">Response</span></span>

<span data-ttu-id="ccde4-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ccde4-132">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="ccde4-133">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="ccde4-133">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="ccde4-134">示例</span><span class="sxs-lookup"><span data-stu-id="ccde4-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccde4-135">请求</span><span class="sxs-lookup"><span data-stu-id="ccde4-135">Request</span></span>

<span data-ttu-id="ccde4-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ccde4-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders_2"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_PartnerSignUp/identityProviders/Facebook-OAUTH/$ref
```

### <a name="response"></a><span data-ttu-id="ccde4-137">响应</span><span class="sxs-lookup"><span data-stu-id="ccde4-137">Response</span></span>

<span data-ttu-id="ccde4-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ccde4-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
