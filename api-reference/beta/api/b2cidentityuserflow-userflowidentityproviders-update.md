---
title: 添加 userFlowIdentityProvider
description: 将 identityProvider 添加到 b2cIdentityUserFlow。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 3c30480e15b836a213a668e0948dcdb3436fbaf1
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401072"
---
# <a name="add-a-userflowidentityprovider"></a><span data-ttu-id="5232c-103">添加 userFlowIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="5232c-103">Add a userFlowIdentityProvider</span></span>

<span data-ttu-id="5232c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5232c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5232c-105">在 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象中添加标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="5232c-105">Add an identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5232c-106">权限</span><span class="sxs-lookup"><span data-stu-id="5232c-106">Permissions</span></span>

<span data-ttu-id="5232c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5232c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5232c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5232c-109">Permission type</span></span>      | <span data-ttu-id="5232c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5232c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5232c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5232c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5232c-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5232c-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="5232c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5232c-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="5232c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5232c-114">Not supported.</span></span>|
|<span data-ttu-id="5232c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5232c-115">Application</span></span>| <span data-ttu-id="5232c-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5232c-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="5232c-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="5232c-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="5232c-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="5232c-118">Global administrator</span></span>
* <span data-ttu-id="5232c-119">外部 ID 用户流管理员</span><span class="sxs-lookup"><span data-stu-id="5232c-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="5232c-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5232c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/b2cUserFlows/{userflow-id}/userflowIdentityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="5232c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5232c-121">Request headers</span></span>

|<span data-ttu-id="5232c-122">名称</span><span class="sxs-lookup"><span data-stu-id="5232c-122">Name</span></span>|<span data-ttu-id="5232c-123">说明</span><span class="sxs-lookup"><span data-stu-id="5232c-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="5232c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5232c-124">Authorization</span></span>|<span data-ttu-id="5232c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5232c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5232c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5232c-127">Content-Type</span></span>|<span data-ttu-id="5232c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5232c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5232c-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5232c-130">Request body</span></span>

<span data-ttu-id="5232c-131">在请求正文中，提供要添加的 `id` [identityProvider](../resources/identityproviderbase.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5232c-131">In the request body, provide a JSON representation with the `id` of the [identityProvider](../resources/identityproviderbase.md) you want to add.</span></span> <span data-ttu-id="5232c-132">有关可用于用户流的标识提供程序详细信息，请参阅 [identityProviders](../resources/identityproviderbase.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="5232c-132">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityproviderbase.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="5232c-133">响应</span><span class="sxs-lookup"><span data-stu-id="5232c-133">Response</span></span>

<span data-ttu-id="5232c-134">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5232c-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="5232c-135">如果失败， `4xx` 将返回包含特定错误详细信息的错误。</span><span class="sxs-lookup"><span data-stu-id="5232c-135">If unsuccessful, a `4xx` error is returned with the specific error details.</span></span>

## <a name="example"></a><span data-ttu-id="5232c-136">示例</span><span class="sxs-lookup"><span data-stu-id="5232c-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="5232c-137">请求</span><span class="sxs-lookup"><span data-stu-id="5232c-137">Request</span></span>

<span data-ttu-id="5232c-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5232c-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_b2cuserflows_userflowIdentityProviders"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/beta/identity/identityProviders/{id}"
}
```

### <a name="response"></a><span data-ttu-id="5232c-139">响应</span><span class="sxs-lookup"><span data-stu-id="5232c-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
