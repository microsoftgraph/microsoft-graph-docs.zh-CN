---
title: 删除 b2cUserFlow
description: 删除 b2cUserFlow 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 35ed189a75bc862df1ae0c3b1936532e133e30ee
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319682"
---
# <a name="delete-b2cuserflow"></a><span data-ttu-id="3f953-103">删除 b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="3f953-103">Delete b2cUserFlow</span></span>

<span data-ttu-id="3f953-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f953-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f953-105">删除 [b2cUserFlow](../resources/b2cuserflows.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3f953-105">Delete a [b2cUserFlow](../resources/b2cuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f953-106">权限</span><span class="sxs-lookup"><span data-stu-id="3f953-106">Permissions</span></span>

<span data-ttu-id="3f953-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3f953-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f953-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f953-109">Permission type</span></span>      | <span data-ttu-id="3f953-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3f953-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f953-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f953-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3f953-112">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="3f953-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="3f953-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f953-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3f953-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f953-114">Not supported.</span></span>|
|<span data-ttu-id="3f953-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f953-115">Application</span></span>|<span data-ttu-id="3f953-116">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="3f953-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="3f953-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="3f953-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="3f953-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="3f953-118">Global administrator</span></span>
* <span data-ttu-id="3f953-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="3f953-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="3f953-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f953-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3f953-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f953-121">Request headers</span></span>

|<span data-ttu-id="3f953-122">名称</span><span class="sxs-lookup"><span data-stu-id="3f953-122">Name</span></span>|<span data-ttu-id="3f953-123">说明</span><span class="sxs-lookup"><span data-stu-id="3f953-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3f953-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f953-124">Authorization</span></span>|<span data-ttu-id="3f953-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3f953-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f953-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f953-127">Request body</span></span>

<span data-ttu-id="3f953-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3f953-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f953-129">响应</span><span class="sxs-lookup"><span data-stu-id="3f953-129">Response</span></span>

<span data-ttu-id="3f953-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="3f953-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3f953-131">示例</span><span class="sxs-lookup"><span data-stu-id="3f953-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f953-132">请求</span><span class="sxs-lookup"><span data-stu-id="3f953-132">Request</span></span>

<span data-ttu-id="3f953-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3f953-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2cUserFlows"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}
```

### <a name="response"></a><span data-ttu-id="3f953-134">响应</span><span class="sxs-lookup"><span data-stu-id="3f953-134">Response</span></span>

<span data-ttu-id="3f953-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3f953-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
