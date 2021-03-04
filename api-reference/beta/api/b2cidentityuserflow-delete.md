---
title: 删除 b2cIdentityUserFlow
description: 删除 b2cIdentityUserFlow 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 11ea70b285f20e281d342e808ad1a15b98041572
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438349"
---
# <a name="delete-b2cidentityuserflow"></a><span data-ttu-id="0e821-103">删除 b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="0e821-103">Delete b2cIdentityUserFlow</span></span>

<span data-ttu-id="0e821-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e821-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e821-105">删除 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0e821-105">Delete a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e821-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0e821-106">Permissions</span></span>

<span data-ttu-id="0e821-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e821-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e821-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e821-109">Permission type</span></span>      | <span data-ttu-id="0e821-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e821-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e821-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e821-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0e821-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e821-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="0e821-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e821-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0e821-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e821-114">Not supported.</span></span>|
|<span data-ttu-id="0e821-115">Application</span><span class="sxs-lookup"><span data-stu-id="0e821-115">Application</span></span>|<span data-ttu-id="0e821-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e821-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="0e821-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="0e821-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="0e821-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="0e821-118">Global administrator</span></span>
* <span data-ttu-id="0e821-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="0e821-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="0e821-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e821-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0e821-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e821-121">Request headers</span></span>

|<span data-ttu-id="0e821-122">名称</span><span class="sxs-lookup"><span data-stu-id="0e821-122">Name</span></span>|<span data-ttu-id="0e821-123">说明</span><span class="sxs-lookup"><span data-stu-id="0e821-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="0e821-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e821-124">Authorization</span></span>|<span data-ttu-id="0e821-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e821-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e821-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e821-127">Request body</span></span>

<span data-ttu-id="0e821-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0e821-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e821-129">响应</span><span class="sxs-lookup"><span data-stu-id="0e821-129">Response</span></span>

<span data-ttu-id="0e821-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0e821-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0e821-131">示例</span><span class="sxs-lookup"><span data-stu-id="0e821-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e821-132">请求</span><span class="sxs-lookup"><span data-stu-id="0e821-132">Request</span></span>

<span data-ttu-id="0e821-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0e821-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0e821-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e821-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2cUserFlows"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="0e821-135">C#</span><span class="sxs-lookup"><span data-stu-id="0e821-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e821-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e821-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e821-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e821-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e821-138">Java</span><span class="sxs-lookup"><span data-stu-id="0e821-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2cuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0e821-139">响应</span><span class="sxs-lookup"><span data-stu-id="0e821-139">Response</span></span>

<span data-ttu-id="0e821-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0e821-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```


