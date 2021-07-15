---
title: 添加 userFlowIdentityProvider
description: 将 identityProvider 添加到 b2cIdentityUserFlow。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: c183cd97377004d60485dcacf0bf372f8957f0b8
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439674"
---
# <a name="add-a-userflowidentityprovider"></a><span data-ttu-id="4aff7-103">添加 userFlowIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="4aff7-103">Add a userFlowIdentityProvider</span></span>

<span data-ttu-id="4aff7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4aff7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4aff7-105">在 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象中添加标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="4aff7-105">Add an identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4aff7-106">权限</span><span class="sxs-lookup"><span data-stu-id="4aff7-106">Permissions</span></span>

<span data-ttu-id="4aff7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4aff7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4aff7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4aff7-109">Permission type</span></span>      | <span data-ttu-id="4aff7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4aff7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4aff7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4aff7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4aff7-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4aff7-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="4aff7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4aff7-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="4aff7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4aff7-114">Not supported.</span></span>|
|<span data-ttu-id="4aff7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4aff7-115">Application</span></span>| <span data-ttu-id="4aff7-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4aff7-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="4aff7-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="4aff7-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="4aff7-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="4aff7-118">Global administrator</span></span>
* <span data-ttu-id="4aff7-119">外部 ID 用户流管理员</span><span class="sxs-lookup"><span data-stu-id="4aff7-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="4aff7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4aff7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/b2cUserFlows/{userflow-id}/userflowIdentityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="4aff7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4aff7-121">Request headers</span></span>

|<span data-ttu-id="4aff7-122">名称</span><span class="sxs-lookup"><span data-stu-id="4aff7-122">Name</span></span>|<span data-ttu-id="4aff7-123">说明</span><span class="sxs-lookup"><span data-stu-id="4aff7-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="4aff7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4aff7-124">Authorization</span></span>|<span data-ttu-id="4aff7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4aff7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4aff7-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4aff7-127">Content-Type</span></span>|<span data-ttu-id="4aff7-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4aff7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4aff7-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="4aff7-130">Request body</span></span>

<span data-ttu-id="4aff7-131">在请求正文中，提供要添加的 `id` [identityProvider](../resources/identityproviderbase.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4aff7-131">In the request body, provide a JSON representation with the `id` of the [identityProvider](../resources/identityproviderbase.md) you want to add.</span></span> <span data-ttu-id="4aff7-132">有关可用于用户流的标识提供程序详细信息，请参阅 [identityProviders](../resources/identityproviderbase.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="4aff7-132">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityproviderbase.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="4aff7-133">响应</span><span class="sxs-lookup"><span data-stu-id="4aff7-133">Response</span></span>

<span data-ttu-id="4aff7-134">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4aff7-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="4aff7-135">如果失败， `4xx` 将返回包含特定错误详细信息的错误。</span><span class="sxs-lookup"><span data-stu-id="4aff7-135">If unsuccessful, a `4xx` error is returned with the specific error details.</span></span>

## <a name="example"></a><span data-ttu-id="4aff7-136">示例</span><span class="sxs-lookup"><span data-stu-id="4aff7-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="4aff7-137">请求</span><span class="sxs-lookup"><span data-stu-id="4aff7-137">Request</span></span>

<span data-ttu-id="4aff7-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4aff7-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4aff7-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="4aff7-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4aff7-140">C#</span><span class="sxs-lookup"><span data-stu-id="4aff7-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2cuserflows-userflowidentityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4aff7-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4aff7-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2cuserflows-userflowidentityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4aff7-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4aff7-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2cuserflows-userflowidentityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4aff7-143">Java</span><span class="sxs-lookup"><span data-stu-id="4aff7-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-b2cuserflows-userflowidentityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4aff7-144">响应</span><span class="sxs-lookup"><span data-stu-id="4aff7-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
