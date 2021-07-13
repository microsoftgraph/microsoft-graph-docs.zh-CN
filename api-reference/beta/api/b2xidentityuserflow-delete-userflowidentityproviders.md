---
title: 删除 userFlowIdentityProvider
description: 从 b2xIdentityUserFlow 中删除 identityProvider。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: f3acd6b37092903050179ebc5377428cec7e2af0
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401066"
---
# <a name="delete-a-userflowidentityprovider"></a><span data-ttu-id="132d2-103">删除 userFlowIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="132d2-103">Delete a userFlowIdentityProvider</span></span>

<span data-ttu-id="132d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="132d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="132d2-105">从 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象中删除标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="132d2-105">Delete an identity provider from a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span> <span data-ttu-id="132d2-106">对于自助注册用户流，值可以是 `Google-OAUTH` 或 `Facebook-OAUTH` 。</span><span class="sxs-lookup"><span data-stu-id="132d2-106">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="permissions"></a><span data-ttu-id="132d2-107">权限</span><span class="sxs-lookup"><span data-stu-id="132d2-107">Permissions</span></span>

<span data-ttu-id="132d2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="132d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="132d2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="132d2-110">Permission type</span></span>      | <span data-ttu-id="132d2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="132d2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="132d2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="132d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="132d2-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="132d2-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="132d2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="132d2-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="132d2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="132d2-115">Not supported.</span></span>|
|<span data-ttu-id="132d2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="132d2-116">Application</span></span>| <span data-ttu-id="132d2-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="132d2-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="132d2-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="132d2-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="132d2-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="132d2-119">Global administrator</span></span>
* <span data-ttu-id="132d2-120">外部 ID 用户流管理员</span><span class="sxs-lookup"><span data-stu-id="132d2-120">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="132d2-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="132d2-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE/identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="132d2-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="132d2-122">Request headers</span></span>

|<span data-ttu-id="132d2-123">名称</span><span class="sxs-lookup"><span data-stu-id="132d2-123">Name</span></span>|<span data-ttu-id="132d2-124">说明</span><span class="sxs-lookup"><span data-stu-id="132d2-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="132d2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="132d2-125">Authorization</span></span>|<span data-ttu-id="132d2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="132d2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="132d2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="132d2-128">Request body</span></span>

<span data-ttu-id="132d2-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="132d2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="132d2-130">响应</span><span class="sxs-lookup"><span data-stu-id="132d2-130">Response</span></span>

<span data-ttu-id="132d2-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="132d2-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="132d2-132">如果失败， `4xx` 将返回包含特定错误详细信息的错误。</span><span class="sxs-lookup"><span data-stu-id="132d2-132">If unsuccessful, a `4xx` error is returned with the specific error details.</span></span>

## <a name="example"></a><span data-ttu-id="132d2-133">示例</span><span class="sxs-lookup"><span data-stu-id="132d2-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="132d2-134">请求</span><span class="sxs-lookup"><span data-stu-id="132d2-134">Request</span></span>

<span data-ttu-id="132d2-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="132d2-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_userflowIdentityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders/{identityProvider-id}/$ref
```

### <a name="response"></a><span data-ttu-id="132d2-136">响应</span><span class="sxs-lookup"><span data-stu-id="132d2-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
