---
title: 删除 b2xIdentityUserFlow
description: 删除 b2xIdentityUserFlow 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 277695339f36c0b3e6d4e00038d001f0dc3760c4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961112"
---
# <a name="delete-b2xidentityuserflow"></a><span data-ttu-id="93823-103">删除 b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="93823-103">Delete b2xIdentityUserFlow</span></span>

<span data-ttu-id="93823-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93823-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93823-105">删除 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="93823-105">Delete a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="93823-106">权限</span><span class="sxs-lookup"><span data-stu-id="93823-106">Permissions</span></span>

<span data-ttu-id="93823-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="93823-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93823-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="93823-109">Permission type</span></span>      | <span data-ttu-id="93823-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="93823-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93823-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93823-111">Delegated (work or school account)</span></span>|<span data-ttu-id="93823-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93823-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="93823-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93823-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="93823-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="93823-114">Not supported.</span></span>|
|<span data-ttu-id="93823-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="93823-115">Application</span></span>|<span data-ttu-id="93823-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93823-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="93823-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="93823-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="93823-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="93823-118">Global administrator</span></span>
* <span data-ttu-id="93823-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="93823-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="93823-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93823-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/b2xUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="93823-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="93823-121">Request headers</span></span>

|<span data-ttu-id="93823-122">名称</span><span class="sxs-lookup"><span data-stu-id="93823-122">Name</span></span>|<span data-ttu-id="93823-123">说明</span><span class="sxs-lookup"><span data-stu-id="93823-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="93823-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="93823-124">Authorization</span></span>|<span data-ttu-id="93823-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="93823-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="93823-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="93823-127">Request body</span></span>

<span data-ttu-id="93823-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="93823-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93823-129">响应</span><span class="sxs-lookup"><span data-stu-id="93823-129">Response</span></span>

<span data-ttu-id="93823-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="93823-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="93823-131">示例</span><span class="sxs-lookup"><span data-stu-id="93823-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="93823-132">请求</span><span class="sxs-lookup"><span data-stu-id="93823-132">Request</span></span>

<span data-ttu-id="93823-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="93823-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="93823-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="93823-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="93823-135">C#</span><span class="sxs-lookup"><span data-stu-id="93823-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93823-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93823-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93823-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93823-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93823-138">Java</span><span class="sxs-lookup"><span data-stu-id="93823-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2xuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="93823-139">响应</span><span class="sxs-lookup"><span data-stu-id="93823-139">Response</span></span>

<span data-ttu-id="93823-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="93823-140">The following is an example of the response.</span></span>

<span data-ttu-id="93823-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="93823-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```


