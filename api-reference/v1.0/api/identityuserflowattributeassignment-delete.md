---
title: 删除 userAttributeAssignment
description: 删除 identityUserFlowAttributeAssignment 对象。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2cf34a4e1da47a0c974585f430fa0d3f85dcf552
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882954"
---
# <a name="delete-userattributeassignment"></a><span data-ttu-id="3e07a-103">删除 userAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="3e07a-103">Delete userAttributeAssignment</span></span>

<span data-ttu-id="3e07a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e07a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e07a-105">删除 [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3e07a-105">Delete an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e07a-106">权限</span><span class="sxs-lookup"><span data-stu-id="3e07a-106">Permissions</span></span>

<span data-ttu-id="3e07a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e07a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e07a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e07a-109">Permission type</span></span>|<span data-ttu-id="3e07a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e07a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e07a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e07a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3e07a-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e07a-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="3e07a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e07a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e07a-114">不支持</span><span class="sxs-lookup"><span data-stu-id="3e07a-114">Not supported</span></span>|
|<span data-ttu-id="3e07a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e07a-115">Application</span></span>|<span data-ttu-id="3e07a-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e07a-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e07a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e07a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3e07a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e07a-118">Request headers</span></span>

|<span data-ttu-id="3e07a-119">名称</span><span class="sxs-lookup"><span data-stu-id="3e07a-119">Name</span></span>|<span data-ttu-id="3e07a-120">说明</span><span class="sxs-lookup"><span data-stu-id="3e07a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3e07a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e07a-121">Authorization</span></span>|<span data-ttu-id="3e07a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3e07a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e07a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e07a-124">Request body</span></span>

<span data-ttu-id="3e07a-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3e07a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e07a-126">响应</span><span class="sxs-lookup"><span data-stu-id="3e07a-126">Response</span></span>

<span data-ttu-id="3e07a-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="3e07a-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3e07a-128">示例</span><span class="sxs-lookup"><span data-stu-id="3e07a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3e07a-129">请求</span><span class="sxs-lookup"><span data-stu-id="3e07a-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_userattributeassignments_from_b2xidentityuserflow"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/City
```

### <a name="response"></a><span data-ttu-id="3e07a-130">响应</span><span class="sxs-lookup"><span data-stu-id="3e07a-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
