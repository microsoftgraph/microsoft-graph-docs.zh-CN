---
title: 从 b2cIdentityUserFlow 中删除 Identityprovider.read.all
description: 从 b2cIdentityUserFlow 中删除 Identityprovider.read.all。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c670adb59f6acf7eb04579f64e80efebb718304b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961244"
---
# <a name="delete-an-identityprovider-from-a-b2cidentityuserflow"></a><span data-ttu-id="82bac-103">从 b2cIdentityUserFlow 中删除 Identityprovider.read.all</span><span class="sxs-lookup"><span data-stu-id="82bac-103">Delete an identityProvider from a b2cIdentityUserFlow</span></span>

<span data-ttu-id="82bac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82bac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82bac-105">从 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象中删除标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="82bac-105">Delete an identity provider from a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span> <span data-ttu-id="82bac-106">有关可用于用户流的标识提供程序的详细信息，请参阅 [identityProviders](../resources/identityprovider.md) API reference。</span><span class="sxs-lookup"><span data-stu-id="82bac-106">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="permissions"></a><span data-ttu-id="82bac-107">权限</span><span class="sxs-lookup"><span data-stu-id="82bac-107">Permissions</span></span>

<span data-ttu-id="82bac-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82bac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82bac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="82bac-110">Permission type</span></span>      | <span data-ttu-id="82bac-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82bac-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82bac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82bac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82bac-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82bac-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="82bac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82bac-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="82bac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="82bac-115">Not supported.</span></span>|
|<span data-ttu-id="82bac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="82bac-116">Application</span></span>| <span data-ttu-id="82bac-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82bac-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="82bac-118">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="82bac-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="82bac-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="82bac-119">Global administrator</span></span>
* <span data-ttu-id="82bac-120">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="82bac-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="82bac-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82bac-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /b2cUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="82bac-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="82bac-122">Request headers</span></span>

|<span data-ttu-id="82bac-123">名称</span><span class="sxs-lookup"><span data-stu-id="82bac-123">Name</span></span>|<span data-ttu-id="82bac-124">说明</span><span class="sxs-lookup"><span data-stu-id="82bac-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="82bac-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="82bac-125">Authorization</span></span>|<span data-ttu-id="82bac-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="82bac-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="82bac-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="82bac-128">Request body</span></span>

<span data-ttu-id="82bac-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="82bac-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82bac-130">响应</span><span class="sxs-lookup"><span data-stu-id="82bac-130">Response</span></span>

<span data-ttu-id="82bac-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="82bac-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="82bac-132">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="82bac-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="82bac-133">示例</span><span class="sxs-lookup"><span data-stu-id="82bac-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="82bac-134">请求</span><span class="sxs-lookup"><span data-stu-id="82bac-134">Request</span></span>

<span data-ttu-id="82bac-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="82bac-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="82bac-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="82bac-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/identityProviders/Facebook-OAUTH/$ref
```
# <a name="c"></a>[<span data-ttu-id="82bac-137">C#</span><span class="sxs-lookup"><span data-stu-id="82bac-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82bac-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82bac-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82bac-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82bac-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="82bac-140">Java</span><span class="sxs-lookup"><span data-stu-id="82bac-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2xuserflows-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="82bac-141">响应</span><span class="sxs-lookup"><span data-stu-id="82bac-141">Response</span></span>

<span data-ttu-id="82bac-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="82bac-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


