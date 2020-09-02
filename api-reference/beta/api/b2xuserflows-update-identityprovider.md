---
title: 将 Identityprovider.read.all 添加到 b2xUserFlow
description: 在 b2xUserFlow 中添加 Identityprovider.read.all。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 792b3ccd9d8020af7139108efd93e0cb430385d7
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329503"
---
# <a name="add-identityprovider-to-a-b2xuserflow"></a><span data-ttu-id="75e09-103">将 Identityprovider.read.all 添加到 b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="75e09-103">Add identityProvider to a b2xUserFlow</span></span>

<span data-ttu-id="75e09-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75e09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75e09-105">更新 [b2xUserFlow](../resources/b2xuserflows.md) 对象中的标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="75e09-105">Update the identity providers in a [b2xUserFlow](../resources/b2xuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="75e09-106">权限</span><span class="sxs-lookup"><span data-stu-id="75e09-106">Permissions</span></span>

<span data-ttu-id="75e09-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75e09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75e09-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="75e09-109">Permission type</span></span>      | <span data-ttu-id="75e09-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="75e09-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75e09-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75e09-111">Delegated (work or school account)</span></span>|<span data-ttu-id="75e09-112">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="75e09-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="75e09-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75e09-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="75e09-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="75e09-114">Not supported.</span></span>|
|<span data-ttu-id="75e09-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="75e09-115">Application</span></span>| <span data-ttu-id="75e09-116">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="75e09-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="75e09-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="75e09-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="75e09-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="75e09-118">Global administrator</span></span>
* <span data-ttu-id="75e09-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="75e09-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="75e09-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75e09-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /b2xUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="75e09-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="75e09-121">Request headers</span></span>

|<span data-ttu-id="75e09-122">名称</span><span class="sxs-lookup"><span data-stu-id="75e09-122">Name</span></span>|<span data-ttu-id="75e09-123">说明</span><span class="sxs-lookup"><span data-stu-id="75e09-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="75e09-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="75e09-124">Authorization</span></span>|<span data-ttu-id="75e09-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="75e09-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="75e09-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="75e09-127">Content-Type</span></span>|<span data-ttu-id="75e09-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="75e09-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75e09-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="75e09-130">Request body</span></span>

<span data-ttu-id="75e09-131">在请求正文中，提供 `id` 要添加的 [IDENTITYPROVIDER.READ.ALL](../resources/identityprovider.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75e09-131">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="75e09-132">对于自助服务注册用户流，值可以是 `Google-OAUTH` 或 `Facebook-OAUTH` 。</span><span class="sxs-lookup"><span data-stu-id="75e09-132">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="response"></a><span data-ttu-id="75e09-133">响应</span><span class="sxs-lookup"><span data-stu-id="75e09-133">Response</span></span>

<span data-ttu-id="75e09-134">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="75e09-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="75e09-135">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="75e09-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="75e09-136">示例</span><span class="sxs-lookup"><span data-stu-id="75e09-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="75e09-137">请求</span><span class="sxs-lookup"><span data-stu-id="75e09-137">Request</span></span>

<span data-ttu-id="75e09-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="75e09-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="75e09-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="75e09-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_b2xuserflows_identityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="75e09-140">C#</span><span class="sxs-lookup"><span data-stu-id="75e09-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-b2xuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75e09-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75e09-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-b2xuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75e09-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75e09-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-b2xuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="75e09-143">响应</span><span class="sxs-lookup"><span data-stu-id="75e09-143">Response</span></span>

<span data-ttu-id="75e09-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="75e09-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
