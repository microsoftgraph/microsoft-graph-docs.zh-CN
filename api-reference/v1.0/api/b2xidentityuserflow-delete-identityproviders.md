---
title: 从 b2xIdentityUserFlow 中删除 identityProvider
description: 从 b2xIdentityUserFlow 中删除 identityProvider。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: eb37182bf72d2e1609c3077df5e4c3a1df4a618e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882992"
---
# <a name="delete-identityprovider-from-b2xidentityuserflow"></a><span data-ttu-id="512af-103">从 b2xIdentityUserFlow 中删除 identityProvider</span><span class="sxs-lookup"><span data-stu-id="512af-103">Delete identityProvider from b2xIdentityUserFlow</span></span>

<span data-ttu-id="512af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="512af-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="512af-105">从 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象中删除标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="512af-105">Delete an identity provider from a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span> <span data-ttu-id="512af-106">对于自助注册用户流，值可以是 `Google-OAUTH` 或 `Facebook-OAUTH` 。</span><span class="sxs-lookup"><span data-stu-id="512af-106">For self-service sign-up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="permissions"></a><span data-ttu-id="512af-107">权限</span><span class="sxs-lookup"><span data-stu-id="512af-107">Permissions</span></span>

<span data-ttu-id="512af-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="512af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="512af-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="512af-110">Permission type</span></span>      | <span data-ttu-id="512af-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="512af-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="512af-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="512af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="512af-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="512af-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="512af-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="512af-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="512af-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="512af-115">Not supported.</span></span>|
|<span data-ttu-id="512af-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="512af-116">Application</span></span>| <span data-ttu-id="512af-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="512af-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="512af-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="512af-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="512af-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="512af-119">Global administrator</span></span>
* <span data-ttu-id="512af-120">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="512af-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="512af-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="512af-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2xUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="512af-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="512af-122">Request headers</span></span>

|<span data-ttu-id="512af-123">名称</span><span class="sxs-lookup"><span data-stu-id="512af-123">Name</span></span>|<span data-ttu-id="512af-124">说明</span><span class="sxs-lookup"><span data-stu-id="512af-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="512af-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="512af-125">Authorization</span></span>|<span data-ttu-id="512af-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="512af-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="512af-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="512af-128">Request body</span></span>

<span data-ttu-id="512af-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="512af-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="512af-130">响应</span><span class="sxs-lookup"><span data-stu-id="512af-130">Response</span></span>

<span data-ttu-id="512af-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="512af-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="512af-132">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="512af-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="512af-133">示例</span><span class="sxs-lookup"><span data-stu-id="512af-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="512af-134">请求</span><span class="sxs-lookup"><span data-stu-id="512af-134">Request</span></span>

<span data-ttu-id="512af-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="512af-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders_2"
}
-->

``` http
DELETE https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_PartnerSignUp/identityProviders/Facebook-OAUTH/$ref
```

### <a name="response"></a><span data-ttu-id="512af-136">响应</span><span class="sxs-lookup"><span data-stu-id="512af-136">Response</span></span>

<span data-ttu-id="512af-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="512af-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
