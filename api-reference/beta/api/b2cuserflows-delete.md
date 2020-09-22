---
title: 删除 b2cUserFlow
description: 删除 b2cUserFlow 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 26e4b244128a8dbd61179197d82d9d83a920b91f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991500"
---
# <a name="delete-b2cuserflow"></a><span data-ttu-id="8646f-103">删除 b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="8646f-103">Delete b2cUserFlow</span></span>

<span data-ttu-id="8646f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8646f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8646f-105">删除 [b2cUserFlow](../resources/b2cuserflows.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8646f-105">Delete a [b2cUserFlow](../resources/b2cuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8646f-106">权限</span><span class="sxs-lookup"><span data-stu-id="8646f-106">Permissions</span></span>

<span data-ttu-id="8646f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8646f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8646f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8646f-109">Permission type</span></span>      | <span data-ttu-id="8646f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8646f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8646f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8646f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8646f-112">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="8646f-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="8646f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8646f-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="8646f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8646f-114">Not supported.</span></span>|
|<span data-ttu-id="8646f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8646f-115">Application</span></span>|<span data-ttu-id="8646f-116">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="8646f-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="8646f-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="8646f-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="8646f-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="8646f-118">Global administrator</span></span>
* <span data-ttu-id="8646f-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="8646f-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="8646f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8646f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8646f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8646f-121">Request headers</span></span>

|<span data-ttu-id="8646f-122">名称</span><span class="sxs-lookup"><span data-stu-id="8646f-122">Name</span></span>|<span data-ttu-id="8646f-123">说明</span><span class="sxs-lookup"><span data-stu-id="8646f-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="8646f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8646f-124">Authorization</span></span>|<span data-ttu-id="8646f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8646f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8646f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8646f-127">Request body</span></span>

<span data-ttu-id="8646f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8646f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8646f-129">响应</span><span class="sxs-lookup"><span data-stu-id="8646f-129">Response</span></span>

<span data-ttu-id="8646f-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8646f-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8646f-131">示例</span><span class="sxs-lookup"><span data-stu-id="8646f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8646f-132">请求</span><span class="sxs-lookup"><span data-stu-id="8646f-132">Request</span></span>

<span data-ttu-id="8646f-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8646f-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8646f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8646f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2cUserFlows"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="8646f-135">C#</span><span class="sxs-lookup"><span data-stu-id="8646f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8646f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8646f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8646f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8646f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8646f-138">响应</span><span class="sxs-lookup"><span data-stu-id="8646f-138">Response</span></span>

<span data-ttu-id="8646f-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8646f-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```


