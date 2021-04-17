---
title: 删除 b2xIdentityUserFlow
description: 删除 b2xIdentityUserFlow 对象。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 7742d2243f79e89b0d1df39e247d97ebff940dcb
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882833"
---
# <a name="delete-b2xidentityuserflow"></a><span data-ttu-id="e8def-103">删除 b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="e8def-103">Delete b2xIdentityUserFlow</span></span>

<span data-ttu-id="e8def-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8def-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e8def-105">删除 [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e8def-105">Delete a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8def-106">权限</span><span class="sxs-lookup"><span data-stu-id="e8def-106">Permissions</span></span>

<span data-ttu-id="e8def-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8def-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8def-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8def-109">Permission type</span></span>      | <span data-ttu-id="e8def-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8def-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8def-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8def-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e8def-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8def-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="e8def-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8def-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e8def-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8def-114">Not supported.</span></span>|
|<span data-ttu-id="e8def-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8def-115">Application</span></span>|<span data-ttu-id="e8def-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8def-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="e8def-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="e8def-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="e8def-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="e8def-118">Global administrator</span></span>
* <span data-ttu-id="e8def-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="e8def-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e8def-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8def-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/b2xUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e8def-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8def-121">Request headers</span></span>

|<span data-ttu-id="e8def-122">名称</span><span class="sxs-lookup"><span data-stu-id="e8def-122">Name</span></span>|<span data-ttu-id="e8def-123">说明</span><span class="sxs-lookup"><span data-stu-id="e8def-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e8def-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8def-124">Authorization</span></span>|<span data-ttu-id="e8def-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e8def-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8def-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8def-127">Request body</span></span>

<span data-ttu-id="e8def-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e8def-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8def-129">响应</span><span class="sxs-lookup"><span data-stu-id="e8def-129">Response</span></span>

<span data-ttu-id="e8def-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e8def-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e8def-131">示例</span><span class="sxs-lookup"><span data-stu-id="e8def-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8def-132">请求</span><span class="sxs-lookup"><span data-stu-id="e8def-132">Request</span></span>

<span data-ttu-id="e8def-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e8def-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows"
}
-->

``` http
DELETE https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner
```

### <a name="response"></a><span data-ttu-id="e8def-134">响应</span><span class="sxs-lookup"><span data-stu-id="e8def-134">Response</span></span>

<span data-ttu-id="e8def-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e8def-135">The following is an example of the response.</span></span>

<span data-ttu-id="e8def-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e8def-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
