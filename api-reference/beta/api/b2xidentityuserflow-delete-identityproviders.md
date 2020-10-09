---
title: 从 b2xIdentityUserFlow 中删除 Identityprovider.read.all
description: 从 b2xIdentityUserFlow 中删除 Identityprovider.read.all。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 751a4a5c351126a47f3a6962e951e0cf6a24b178
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406273"
---
# <a name="delete-identityprovider-from-b2xidentityuserflow"></a><span data-ttu-id="60b7d-103">从 b2xIdentityUserFlow 中删除 Identityprovider.read.all</span><span class="sxs-lookup"><span data-stu-id="60b7d-103">Delete identityProvider from b2xIdentityUserFlow</span></span>

<span data-ttu-id="60b7d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60b7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60b7d-105">从 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象中删除标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="60b7d-105">Delete an identity provider from a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span> <span data-ttu-id="60b7d-106">对于自助服务注册用户流，值可以是 `Google-OAUTH` 或 `Facebook-OAUTH` 。</span><span class="sxs-lookup"><span data-stu-id="60b7d-106">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="permissions"></a><span data-ttu-id="60b7d-107">权限</span><span class="sxs-lookup"><span data-stu-id="60b7d-107">Permissions</span></span>

<span data-ttu-id="60b7d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60b7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60b7d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="60b7d-110">Permission type</span></span>      | <span data-ttu-id="60b7d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="60b7d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60b7d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60b7d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="60b7d-113">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="60b7d-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="60b7d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60b7d-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="60b7d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="60b7d-115">Not supported.</span></span>|
|<span data-ttu-id="60b7d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="60b7d-116">Application</span></span>| <span data-ttu-id="60b7d-117">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="60b7d-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="60b7d-118">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="60b7d-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="60b7d-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="60b7d-119">Global administrator</span></span>
* <span data-ttu-id="60b7d-120">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="60b7d-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="60b7d-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60b7d-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /b2xUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="60b7d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="60b7d-122">Request headers</span></span>

|<span data-ttu-id="60b7d-123">名称</span><span class="sxs-lookup"><span data-stu-id="60b7d-123">Name</span></span>|<span data-ttu-id="60b7d-124">说明</span><span class="sxs-lookup"><span data-stu-id="60b7d-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="60b7d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="60b7d-125">Authorization</span></span>|<span data-ttu-id="60b7d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="60b7d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60b7d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="60b7d-128">Request body</span></span>

<span data-ttu-id="60b7d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="60b7d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60b7d-130">响应</span><span class="sxs-lookup"><span data-stu-id="60b7d-130">Response</span></span>

<span data-ttu-id="60b7d-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="60b7d-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="60b7d-132">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="60b7d-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="60b7d-133">示例</span><span class="sxs-lookup"><span data-stu-id="60b7d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="60b7d-134">请求</span><span class="sxs-lookup"><span data-stu-id="60b7d-134">Request</span></span>

<span data-ttu-id="60b7d-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="60b7d-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="60b7d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="60b7d-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_PartnerSignUp/identityProviders/Facebook-OAUTH/$ref
```
# <a name="c"></a>[<span data-ttu-id="60b7d-137">C#</span><span class="sxs-lookup"><span data-stu-id="60b7d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60b7d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60b7d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60b7d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60b7d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="60b7d-140">响应</span><span class="sxs-lookup"><span data-stu-id="60b7d-140">Response</span></span>

<span data-ttu-id="60b7d-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="60b7d-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


