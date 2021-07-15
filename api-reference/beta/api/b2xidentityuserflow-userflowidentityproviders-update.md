---
title: 更新 userFlowIdentityProvider
description: 更新 b2xIdentityUserFlow 中的 identityProvider。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 4b0640cd6843873d720ddc6547e15beb89f7f0f8
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439525"
---
# <a name="update-a-userflowidentityprovider"></a><span data-ttu-id="4c062-103">更新 userFlowIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="4c062-103">Update a userFlowIdentityProvider</span></span>

<span data-ttu-id="4c062-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c062-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c062-105">更新 [b2xIdentityUserFlow 对象中的标识](../resources/b2xidentityuserflow.md) 提供程序。</span><span class="sxs-lookup"><span data-stu-id="4c062-105">Update an identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c062-106">权限</span><span class="sxs-lookup"><span data-stu-id="4c062-106">Permissions</span></span>

<span data-ttu-id="4c062-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4c062-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c062-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c062-109">Permission type</span></span>      | <span data-ttu-id="4c062-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4c062-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c062-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c062-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4c062-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c062-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="4c062-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c062-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="4c062-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c062-114">Not supported.</span></span>|
|<span data-ttu-id="4c062-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c062-115">Application</span></span>| <span data-ttu-id="4c062-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c062-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="4c062-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="4c062-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="4c062-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="4c062-118">Global administrator</span></span>
* <span data-ttu-id="4c062-119">外部 ID 用户流管理员</span><span class="sxs-lookup"><span data-stu-id="4c062-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="4c062-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c062-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="4c062-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4c062-121">Request headers</span></span>

|<span data-ttu-id="4c062-122">名称</span><span class="sxs-lookup"><span data-stu-id="4c062-122">Name</span></span>|<span data-ttu-id="4c062-123">说明</span><span class="sxs-lookup"><span data-stu-id="4c062-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="4c062-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c062-124">Authorization</span></span>|<span data-ttu-id="4c062-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4c062-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4c062-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c062-127">Content-Type</span></span>|<span data-ttu-id="4c062-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4c062-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c062-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c062-130">Request body</span></span>

<span data-ttu-id="4c062-131">在请求正文中，提供要添加的 `id` [identityProvider](../resources/identityproviderbase.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c062-131">In the request body, provide a JSON representation with the `id` of the [identityProvider](../resources/identityproviderbase.md) you want to add.</span></span> <span data-ttu-id="4c062-132">对于自助注册用户流，值可以是 `Google-OAUTH` 或 `Facebook-OAUTH` 。</span><span class="sxs-lookup"><span data-stu-id="4c062-132">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="response"></a><span data-ttu-id="4c062-133">响应</span><span class="sxs-lookup"><span data-stu-id="4c062-133">Response</span></span>

<span data-ttu-id="4c062-134">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4c062-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="4c062-135">如果失败， `4xx` 将返回包含特定错误详细信息的错误。</span><span class="sxs-lookup"><span data-stu-id="4c062-135">If unsuccessful, a `4xx` error is returned with the specific error details.</span></span>

## <a name="example"></a><span data-ttu-id="4c062-136">示例</span><span class="sxs-lookup"><span data-stu-id="4c062-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c062-137">请求</span><span class="sxs-lookup"><span data-stu-id="4c062-137">Request</span></span>

<span data-ttu-id="4c062-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4c062-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4c062-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c062-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_b2xuserflows_userflowidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Test/userflowIdentityProviders/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test"
}
```
# <a name="c"></a>[<span data-ttu-id="4c062-140">C#</span><span class="sxs-lookup"><span data-stu-id="4c062-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2xuserflows-userflowidentityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c062-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c062-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2xuserflows-userflowidentityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c062-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c062-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2xuserflows-userflowidentityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c062-143">Java</span><span class="sxs-lookup"><span data-stu-id="4c062-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-b2xuserflows-userflowidentityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4c062-144">响应</span><span class="sxs-lookup"><span data-stu-id="4c062-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
