---
title: 删除 userFlowIdentityProvider
description: 从 b2xIdentityUserFlow 中删除 identityProvider。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 85fff2d0fab5d9d098aa7cae780c99faece3916f
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439651"
---
# <a name="delete-a-userflowidentityprovider"></a><span data-ttu-id="25e05-103">删除 userFlowIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="25e05-103">Delete a userFlowIdentityProvider</span></span>

<span data-ttu-id="25e05-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25e05-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25e05-105">从 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象中删除标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="25e05-105">Delete an identity provider from a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span> <span data-ttu-id="25e05-106">对于自助注册用户流，值可以是 `Google-OAUTH` 或 `Facebook-OAUTH` 。</span><span class="sxs-lookup"><span data-stu-id="25e05-106">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="permissions"></a><span data-ttu-id="25e05-107">权限</span><span class="sxs-lookup"><span data-stu-id="25e05-107">Permissions</span></span>

<span data-ttu-id="25e05-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25e05-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25e05-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="25e05-110">Permission type</span></span>      | <span data-ttu-id="25e05-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25e05-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25e05-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25e05-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25e05-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25e05-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="25e05-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25e05-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="25e05-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="25e05-115">Not supported.</span></span>|
|<span data-ttu-id="25e05-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="25e05-116">Application</span></span>| <span data-ttu-id="25e05-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25e05-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="25e05-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="25e05-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="25e05-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="25e05-119">Global administrator</span></span>
* <span data-ttu-id="25e05-120">外部 ID 用户流管理员</span><span class="sxs-lookup"><span data-stu-id="25e05-120">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="25e05-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25e05-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE/identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="25e05-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="25e05-122">Request headers</span></span>

|<span data-ttu-id="25e05-123">名称</span><span class="sxs-lookup"><span data-stu-id="25e05-123">Name</span></span>|<span data-ttu-id="25e05-124">说明</span><span class="sxs-lookup"><span data-stu-id="25e05-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="25e05-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="25e05-125">Authorization</span></span>|<span data-ttu-id="25e05-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="25e05-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="25e05-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="25e05-128">Request body</span></span>

<span data-ttu-id="25e05-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="25e05-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25e05-130">响应</span><span class="sxs-lookup"><span data-stu-id="25e05-130">Response</span></span>

<span data-ttu-id="25e05-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="25e05-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="25e05-132">如果失败， `4xx` 将返回包含特定错误详细信息的错误。</span><span class="sxs-lookup"><span data-stu-id="25e05-132">If unsuccessful, a `4xx` error is returned with the specific error details.</span></span>

## <a name="example"></a><span data-ttu-id="25e05-133">示例</span><span class="sxs-lookup"><span data-stu-id="25e05-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="25e05-134">请求</span><span class="sxs-lookup"><span data-stu-id="25e05-134">Request</span></span>

<span data-ttu-id="25e05-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="25e05-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="25e05-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="25e05-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_userflowIdentityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders/{identityProvider-id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="25e05-137">C#</span><span class="sxs-lookup"><span data-stu-id="25e05-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-userflowidentityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25e05-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25e05-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-userflowidentityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25e05-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25e05-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-userflowidentityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="25e05-140">Java</span><span class="sxs-lookup"><span data-stu-id="25e05-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2xuserflows-userflowidentityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="25e05-141">响应</span><span class="sxs-lookup"><span data-stu-id="25e05-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
