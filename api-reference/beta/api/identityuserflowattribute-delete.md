---
title: 删除 identityUserFlowAttribute
description: 删除 identityUserFlowAttribute。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 76eaa73ad22a2e418caf9bff7904422c16c01037
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742358"
---
# <a name="delete-identityuserflowattribute"></a><span data-ttu-id="0795a-103">删除 identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="0795a-103">Delete identityUserFlowAttribute</span></span>

<span data-ttu-id="0795a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0795a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0795a-105">删除 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)。</span><span class="sxs-lookup"><span data-stu-id="0795a-105">Delete an [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="0795a-106">仅可删除自定义用户流属性。</span><span class="sxs-lookup"><span data-stu-id="0795a-106">Only custom user flow attributes can be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="0795a-107">权限</span><span class="sxs-lookup"><span data-stu-id="0795a-107">Permissions</span></span>

<span data-ttu-id="0795a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0795a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0795a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0795a-110">Permission type</span></span>      | <span data-ttu-id="0795a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0795a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0795a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0795a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0795a-113">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="0795a-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="0795a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0795a-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0795a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0795a-115">Not supported.</span></span>|
|<span data-ttu-id="0795a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0795a-116">Application</span></span>|<span data-ttu-id="0795a-117">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="0795a-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="0795a-118">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="0795a-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="0795a-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="0795a-119">Global administrator</span></span>
* <span data-ttu-id="0795a-120">外部标识用户流属性管理员</span><span class="sxs-lookup"><span data-stu-id="0795a-120">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="0795a-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0795a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0795a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="0795a-122">Request headers</span></span>

|<span data-ttu-id="0795a-123">名称</span><span class="sxs-lookup"><span data-stu-id="0795a-123">Name</span></span>|<span data-ttu-id="0795a-124">说明</span><span class="sxs-lookup"><span data-stu-id="0795a-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="0795a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0795a-125">Authorization</span></span>|<span data-ttu-id="0795a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0795a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0795a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0795a-128">Request body</span></span>

<span data-ttu-id="0795a-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0795a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0795a-130">响应</span><span class="sxs-lookup"><span data-stu-id="0795a-130">Response</span></span>

<span data-ttu-id="0795a-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0795a-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0795a-132">示例</span><span class="sxs-lookup"><span data-stu-id="0795a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0795a-133">请求</span><span class="sxs-lookup"><span data-stu-id="0795a-133">Request</span></span>

<span data-ttu-id="0795a-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0795a-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_userFlowAttributes"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/userFlowAttributes/{id}
```

### <a name="response"></a><span data-ttu-id="0795a-135">响应</span><span class="sxs-lookup"><span data-stu-id="0795a-135">Response</span></span>

<span data-ttu-id="0795a-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0795a-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
