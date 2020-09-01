---
title: 删除 b2xUserFlow
description: 删除 b2xUserFlow 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2e408c96d70efc04168954cbe82448a9e6a71cd1
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319669"
---
# <a name="delete-b2xuserflow"></a><span data-ttu-id="f2b7e-103">删除 b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="f2b7e-103">Delete b2xUserFlow</span></span>

<span data-ttu-id="f2b7e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2b7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2b7e-105">删除 [b2xUserFlow](../resources/b2xuserflows.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2b7e-105">Delete a [b2xUserFlow](../resources/b2xuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2b7e-106">权限</span><span class="sxs-lookup"><span data-stu-id="f2b7e-106">Permissions</span></span>

<span data-ttu-id="f2b7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2b7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2b7e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2b7e-109">Permission type</span></span>      | <span data-ttu-id="f2b7e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2b7e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2b7e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2b7e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2b7e-112">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="f2b7e-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="f2b7e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2b7e-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f2b7e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2b7e-114">Not supported.</span></span>|
|<span data-ttu-id="f2b7e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2b7e-115">Application</span></span>|<span data-ttu-id="f2b7e-116">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="f2b7e-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="f2b7e-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="f2b7e-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f2b7e-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="f2b7e-118">Global administrator</span></span>
* <span data-ttu-id="f2b7e-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="f2b7e-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f2b7e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2b7e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/b2xUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f2b7e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2b7e-121">Request headers</span></span>

|<span data-ttu-id="f2b7e-122">名称</span><span class="sxs-lookup"><span data-stu-id="f2b7e-122">Name</span></span>|<span data-ttu-id="f2b7e-123">说明</span><span class="sxs-lookup"><span data-stu-id="f2b7e-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f2b7e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2b7e-124">Authorization</span></span>|<span data-ttu-id="f2b7e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2b7e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2b7e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2b7e-127">Request body</span></span>

<span data-ttu-id="f2b7e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f2b7e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2b7e-129">响应</span><span class="sxs-lookup"><span data-stu-id="f2b7e-129">Response</span></span>

<span data-ttu-id="f2b7e-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f2b7e-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f2b7e-131">示例</span><span class="sxs-lookup"><span data-stu-id="f2b7e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2b7e-132">请求</span><span class="sxs-lookup"><span data-stu-id="f2b7e-132">Request</span></span>

<span data-ttu-id="f2b7e-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f2b7e-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}
```

### <a name="response"></a><span data-ttu-id="f2b7e-134">响应</span><span class="sxs-lookup"><span data-stu-id="f2b7e-134">Response</span></span>

<span data-ttu-id="f2b7e-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f2b7e-135">The following is an example of the response.</span></span>

<span data-ttu-id="f2b7e-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f2b7e-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
