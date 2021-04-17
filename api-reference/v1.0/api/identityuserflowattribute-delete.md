---
title: 删除 identityUserFlowAttribute
description: 删除 identityUserFlowAttribute。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: c5289130cb54ca68889cb5875d6277fe73de1e09
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882427"
---
# <a name="delete-identityuserflowattribute"></a><span data-ttu-id="74927-103">删除 identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="74927-103">Delete identityUserFlowAttribute</span></span>

<span data-ttu-id="74927-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74927-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74927-105">删除 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)。</span><span class="sxs-lookup"><span data-stu-id="74927-105">Delete an [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="74927-106">只能删除自定义用户流属性。</span><span class="sxs-lookup"><span data-stu-id="74927-106">Only custom user flow attributes can be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="74927-107">权限</span><span class="sxs-lookup"><span data-stu-id="74927-107">Permissions</span></span>

<span data-ttu-id="74927-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74927-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74927-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="74927-110">Permission type</span></span>      | <span data-ttu-id="74927-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74927-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74927-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74927-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74927-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74927-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="74927-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74927-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="74927-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="74927-115">Not supported.</span></span>|
|<span data-ttu-id="74927-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="74927-116">Application</span></span>|<span data-ttu-id="74927-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74927-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="74927-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="74927-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="74927-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="74927-119">Global administrator</span></span>
* <span data-ttu-id="74927-120">外部标识用户流属性管理员</span><span class="sxs-lookup"><span data-stu-id="74927-120">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="74927-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74927-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="74927-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="74927-122">Request headers</span></span>

|<span data-ttu-id="74927-123">名称</span><span class="sxs-lookup"><span data-stu-id="74927-123">Name</span></span>|<span data-ttu-id="74927-124">说明</span><span class="sxs-lookup"><span data-stu-id="74927-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="74927-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="74927-125">Authorization</span></span>|<span data-ttu-id="74927-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="74927-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="74927-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="74927-128">Request body</span></span>

<span data-ttu-id="74927-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="74927-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74927-130">响应</span><span class="sxs-lookup"><span data-stu-id="74927-130">Response</span></span>

<span data-ttu-id="74927-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="74927-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="74927-132">示例</span><span class="sxs-lookup"><span data-stu-id="74927-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="74927-133">请求</span><span class="sxs-lookup"><span data-stu-id="74927-133">Request</span></span>

<span data-ttu-id="74927-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="74927-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_userFlowAttributes"
}
-->

``` http
DELETE https://graph.microsoft.com/v1.0/identity/userFlowAttributes/extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby
```

### <a name="response"></a><span data-ttu-id="74927-135">响应</span><span class="sxs-lookup"><span data-stu-id="74927-135">Response</span></span>

<span data-ttu-id="74927-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="74927-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
