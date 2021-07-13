---
title: '将 identityProvider 添加到 b2cIdentityUserFlow (弃) '
description: '将 identityProvider 添加到 b2cIdentityUserFlow。  (已弃) '
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 9b213dd0255984b0ffe99270ec5fa7f69558aabb
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400962"
---
# <a name="add-identityprovider-to-a-b2cidentityuserflow-deprecated"></a><span data-ttu-id="dab9e-104">将 identityProvider 添加到 b2cIdentityUserFlow (弃) </span><span class="sxs-lookup"><span data-stu-id="dab9e-104">Add identityProvider to a b2cIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="dab9e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dab9e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="dab9e-106">在 [b2cIdentityUserFlow 对象中添加标识](../resources/b2cidentityuserflow.md) 提供程序。</span><span class="sxs-lookup"><span data-stu-id="dab9e-106">Add identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dab9e-107">权限</span><span class="sxs-lookup"><span data-stu-id="dab9e-107">Permissions</span></span>

<span data-ttu-id="dab9e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dab9e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dab9e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dab9e-110">Permission type</span></span>      | <span data-ttu-id="dab9e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dab9e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dab9e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dab9e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dab9e-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dab9e-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="dab9e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dab9e-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="dab9e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dab9e-115">Not supported.</span></span>|
|<span data-ttu-id="dab9e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dab9e-116">Application</span></span>| <span data-ttu-id="dab9e-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dab9e-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="dab9e-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="dab9e-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="dab9e-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="dab9e-119">Global administrator</span></span>
* <span data-ttu-id="dab9e-120">外部标识用户Flow管理员</span><span class="sxs-lookup"><span data-stu-id="dab9e-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="dab9e-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dab9e-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2cUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="dab9e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="dab9e-122">Request headers</span></span>

|<span data-ttu-id="dab9e-123">名称</span><span class="sxs-lookup"><span data-stu-id="dab9e-123">Name</span></span>|<span data-ttu-id="dab9e-124">说明</span><span class="sxs-lookup"><span data-stu-id="dab9e-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="dab9e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="dab9e-125">Authorization</span></span>|<span data-ttu-id="dab9e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dab9e-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="dab9e-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dab9e-128">Content-Type</span></span>|<span data-ttu-id="dab9e-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="dab9e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dab9e-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="dab9e-131">Request body</span></span>

<span data-ttu-id="dab9e-132">在请求正文中，提供要添加的 `id` [identityProvider](../resources/identityprovider.md) 的 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dab9e-132">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="dab9e-133">有关可用于用户流的标识提供程序详细信息，请参阅 [identityProviders](../resources/identityprovider.md) API 参考。</span><span class="sxs-lookup"><span data-stu-id="dab9e-133">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="response"></a><span data-ttu-id="dab9e-134">响应</span><span class="sxs-lookup"><span data-stu-id="dab9e-134">Response</span></span>

<span data-ttu-id="dab9e-135">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="dab9e-135">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="dab9e-136">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="dab9e-136">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="dab9e-137">示例</span><span class="sxs-lookup"><span data-stu-id="dab9e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="dab9e-138">请求</span><span class="sxs-lookup"><span data-stu-id="dab9e-138">Request</span></span>

<span data-ttu-id="dab9e-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dab9e-139">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_b2cuserflows_identityprovider"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}"
}
```

### <a name="response"></a><span data-ttu-id="dab9e-140">响应</span><span class="sxs-lookup"><span data-stu-id="dab9e-140">Response</span></span>

<span data-ttu-id="dab9e-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dab9e-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
