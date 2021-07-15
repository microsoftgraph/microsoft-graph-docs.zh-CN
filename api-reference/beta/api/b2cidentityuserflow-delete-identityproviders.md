---
title: '从 b2cIdentityUserFlow 中删除 identityProvider (弃) '
description: '从 b2cIdentityUserFlow 中删除 identityProvider。  (已弃) '
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 64a72b0d286ff9e794d8ca654d498ee95f1a52de
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439810"
---
# <a name="delete-an-identityprovider-from-a-b2cidentityuserflow-deprecated"></a><span data-ttu-id="7f2ee-104">从 b2cIdentityUserFlow 中删除已弃 (identityProvider) </span><span class="sxs-lookup"><span data-stu-id="7f2ee-104">Delete an identityProvider from a b2cIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="7f2ee-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f2ee-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="7f2ee-106">从 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象中删除标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="7f2ee-106">Delete an identity provider from a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span> <span data-ttu-id="7f2ee-107">有关可用于用户流的标识提供程序详细信息，请参阅 [identityProviders](../resources/identityprovider.md) API 参考。</span><span class="sxs-lookup"><span data-stu-id="7f2ee-107">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f2ee-108">权限</span><span class="sxs-lookup"><span data-stu-id="7f2ee-108">Permissions</span></span>

<span data-ttu-id="7f2ee-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f2ee-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f2ee-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f2ee-111">Permission type</span></span>      | <span data-ttu-id="7f2ee-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f2ee-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f2ee-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f2ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f2ee-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f2ee-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="7f2ee-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f2ee-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="7f2ee-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f2ee-116">Not supported.</span></span>|
|<span data-ttu-id="7f2ee-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f2ee-117">Application</span></span>| <span data-ttu-id="7f2ee-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f2ee-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="7f2ee-119">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="7f2ee-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="7f2ee-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="7f2ee-120">Global administrator</span></span>
* <span data-ttu-id="7f2ee-121">外部标识用户Flow管理员</span><span class="sxs-lookup"><span data-stu-id="7f2ee-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="7f2ee-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f2ee-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2cUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="7f2ee-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f2ee-123">Request headers</span></span>

|<span data-ttu-id="7f2ee-124">名称</span><span class="sxs-lookup"><span data-stu-id="7f2ee-124">Name</span></span>|<span data-ttu-id="7f2ee-125">说明</span><span class="sxs-lookup"><span data-stu-id="7f2ee-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="7f2ee-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f2ee-126">Authorization</span></span>|<span data-ttu-id="7f2ee-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7f2ee-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f2ee-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f2ee-129">Request body</span></span>

<span data-ttu-id="7f2ee-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7f2ee-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f2ee-131">响应</span><span class="sxs-lookup"><span data-stu-id="7f2ee-131">Response</span></span>

<span data-ttu-id="7f2ee-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7f2ee-132">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="7f2ee-133">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="7f2ee-133">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="7f2ee-134">示例</span><span class="sxs-lookup"><span data-stu-id="7f2ee-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f2ee-135">请求</span><span class="sxs-lookup"><span data-stu-id="7f2ee-135">Request</span></span>

<span data-ttu-id="7f2ee-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7f2ee-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7f2ee-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f2ee-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders_1"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/identityProviders/Facebook-OAUTH/$ref
```
# <a name="c"></a>[<span data-ttu-id="7f2ee-138">C#</span><span class="sxs-lookup"><span data-stu-id="7f2ee-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-identityproviders-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f2ee-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f2ee-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-identityproviders-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f2ee-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f2ee-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-identityproviders-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f2ee-141">Java</span><span class="sxs-lookup"><span data-stu-id="7f2ee-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2xuserflows-identityproviders-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7f2ee-142">响应</span><span class="sxs-lookup"><span data-stu-id="7f2ee-142">Response</span></span>

<span data-ttu-id="7f2ee-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7f2ee-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
