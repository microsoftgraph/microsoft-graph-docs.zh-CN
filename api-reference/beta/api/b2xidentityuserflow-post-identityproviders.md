---
title: '将 identityProvider 添加到 b2xIdentityUserFlow (弃) '
description: 在 b2xIdentityUserFlow 中添加 identityProvider (弃) 。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 60309219aa24ad4d2aee58b877a324ce1d32aa8b
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400906"
---
# <a name="add-identityprovider-to-a-b2xidentityuserflow-deprecated"></a><span data-ttu-id="eba83-103">将 identityProvider 添加到 b2xIdentityUserFlow (弃) </span><span class="sxs-lookup"><span data-stu-id="eba83-103">Add identityProvider to a b2xIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="eba83-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eba83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="eba83-105">更新 [b2xIdentityUserFlow 对象中的标识](../resources/b2xidentityuserflow.md) 提供程序。</span><span class="sxs-lookup"><span data-stu-id="eba83-105">Update the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eba83-106">权限</span><span class="sxs-lookup"><span data-stu-id="eba83-106">Permissions</span></span>

<span data-ttu-id="eba83-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eba83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eba83-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="eba83-109">Permission type</span></span>      | <span data-ttu-id="eba83-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eba83-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eba83-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eba83-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eba83-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eba83-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="eba83-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eba83-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="eba83-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="eba83-114">Not supported.</span></span>|
|<span data-ttu-id="eba83-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="eba83-115">Application</span></span>| <span data-ttu-id="eba83-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eba83-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="eba83-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="eba83-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="eba83-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="eba83-118">Global administrator</span></span>
* <span data-ttu-id="eba83-119">外部标识用户Flow管理员</span><span class="sxs-lookup"><span data-stu-id="eba83-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="eba83-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eba83-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="eba83-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="eba83-121">Request headers</span></span>

|<span data-ttu-id="eba83-122">名称</span><span class="sxs-lookup"><span data-stu-id="eba83-122">Name</span></span>|<span data-ttu-id="eba83-123">说明</span><span class="sxs-lookup"><span data-stu-id="eba83-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="eba83-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="eba83-124">Authorization</span></span>|<span data-ttu-id="eba83-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eba83-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="eba83-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eba83-127">Content-Type</span></span>|<span data-ttu-id="eba83-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="eba83-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eba83-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="eba83-130">Request body</span></span>

<span data-ttu-id="eba83-131">在请求正文中，提供要添加的 `id` [identityProvider](../resources/identityprovider.md) 的 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eba83-131">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="eba83-132">对于自助注册用户流，值可以是 `Google-OAUTH` 或 `Facebook-OAUTH` 。</span><span class="sxs-lookup"><span data-stu-id="eba83-132">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="response"></a><span data-ttu-id="eba83-133">响应</span><span class="sxs-lookup"><span data-stu-id="eba83-133">Response</span></span>

<span data-ttu-id="eba83-134">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="eba83-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="eba83-135">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="eba83-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="eba83-136">示例</span><span class="sxs-lookup"><span data-stu-id="eba83-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="eba83-137">请求</span><span class="sxs-lookup"><span data-stu-id="eba83-137">Request</span></span>

<span data-ttu-id="eba83-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="eba83-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_b2xuserflows_identityprovider"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}"
}
```

### <a name="response"></a><span data-ttu-id="eba83-139">响应</span><span class="sxs-lookup"><span data-stu-id="eba83-139">Response</span></span>

<span data-ttu-id="eba83-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="eba83-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
