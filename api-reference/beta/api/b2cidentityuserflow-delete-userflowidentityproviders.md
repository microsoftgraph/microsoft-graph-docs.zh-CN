---
title: 删除 userflowidentityproviders
description: 从 b2cIdentityUserFlow 中删除 identityProvider。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 2f8f6f59ea2fcad737dc5fae9bc60d91ec467b31
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439803"
---
# <a name="delete-a-userflowidentityproviders"></a><span data-ttu-id="1cfb8-103">删除 userflowidentityproviders</span><span class="sxs-lookup"><span data-stu-id="1cfb8-103">Delete a userflowidentityproviders</span></span>

<span data-ttu-id="1cfb8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cfb8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cfb8-105">从 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象中删除标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="1cfb8-105">Delete an identity provider from a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span> <span data-ttu-id="1cfb8-106">有关可用于用户流的标识提供程序详细信息，请参阅 [identityProviders](../resources/identityproviderbase.md) API 参考。</span><span class="sxs-lookup"><span data-stu-id="1cfb8-106">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityproviderbase.md) API reference.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cfb8-107">权限</span><span class="sxs-lookup"><span data-stu-id="1cfb8-107">Permissions</span></span>

<span data-ttu-id="1cfb8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1cfb8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cfb8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1cfb8-110">Permission type</span></span>      | <span data-ttu-id="1cfb8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1cfb8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cfb8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1cfb8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1cfb8-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cfb8-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="1cfb8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1cfb8-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="1cfb8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1cfb8-115">Not supported.</span></span>|
|<span data-ttu-id="1cfb8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1cfb8-116">Application</span></span>| <span data-ttu-id="1cfb8-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cfb8-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="1cfb8-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="1cfb8-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="1cfb8-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="1cfb8-119">Global administrator</span></span>
* <span data-ttu-id="1cfb8-120">外部 ID 用户流管理员</span><span class="sxs-lookup"><span data-stu-id="1cfb8-120">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="1cfb8-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1cfb8-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2cUserFlows/{userflow-id}/userflowIdentityProviders/{identityProvider-id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="1cfb8-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1cfb8-122">Request headers</span></span>

|<span data-ttu-id="1cfb8-123">名称</span><span class="sxs-lookup"><span data-stu-id="1cfb8-123">Name</span></span>|<span data-ttu-id="1cfb8-124">说明</span><span class="sxs-lookup"><span data-stu-id="1cfb8-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="1cfb8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cfb8-125">Authorization</span></span>|<span data-ttu-id="1cfb8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1cfb8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cfb8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1cfb8-128">Request body</span></span>

<span data-ttu-id="1cfb8-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1cfb8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cfb8-130">响应</span><span class="sxs-lookup"><span data-stu-id="1cfb8-130">Response</span></span>

<span data-ttu-id="1cfb8-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1cfb8-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="1cfb8-132">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="1cfb8-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="1cfb8-133">示例</span><span class="sxs-lookup"><span data-stu-id="1cfb8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1cfb8-134">请求</span><span class="sxs-lookup"><span data-stu-id="1cfb8-134">Request</span></span>

<span data-ttu-id="1cfb8-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1cfb8-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1cfb8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1cfb8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_userflowIdentityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders/MSA-OIDC/$ref
```
# <a name="c"></a>[<span data-ttu-id="1cfb8-137">C#</span><span class="sxs-lookup"><span data-stu-id="1cfb8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-userflowidentityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1cfb8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1cfb8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-userflowidentityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1cfb8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1cfb8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-userflowidentityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1cfb8-140">Java</span><span class="sxs-lookup"><span data-stu-id="1cfb8-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2xuserflows-userflowidentityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1cfb8-141">响应</span><span class="sxs-lookup"><span data-stu-id="1cfb8-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
