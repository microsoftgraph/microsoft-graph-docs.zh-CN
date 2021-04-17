---
title: identityUserFlowAttributeAssignment：setOrder
description: 设置在用户流中收集的 identityUserFlowAttributeAssignments 的顺序。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2f066bc84a2938734776c4271022cb4756ac1620
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882807"
---
# <a name="identityuserflowattributeassignment-setorder"></a><span data-ttu-id="5469c-103">identityUserFlowAttributeAssignment：setOrder</span><span class="sxs-lookup"><span data-stu-id="5469c-103">identityUserFlowAttributeAssignment: setOrder</span></span>

<span data-ttu-id="5469c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5469c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5469c-105">设置在用户流中收集的 identityUserFlowAttributeAssignments 的顺序。</span><span class="sxs-lookup"><span data-stu-id="5469c-105">Set the order of identityUserFlowAttributeAssignments being collected within a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="5469c-106">权限</span><span class="sxs-lookup"><span data-stu-id="5469c-106">Permissions</span></span>

<span data-ttu-id="5469c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5469c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5469c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5469c-109">Permission type</span></span>|<span data-ttu-id="5469c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5469c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5469c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5469c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5469c-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5469c-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="5469c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5469c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5469c-114">不支持</span><span class="sxs-lookup"><span data-stu-id="5469c-114">Not supported</span></span>|
|<span data-ttu-id="5469c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5469c-115">Application</span></span>|<span data-ttu-id="5469c-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5469c-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5469c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5469c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/setOrder
```

## <a name="request-headers"></a><span data-ttu-id="5469c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5469c-118">Request headers</span></span>

|<span data-ttu-id="5469c-119">名称</span><span class="sxs-lookup"><span data-stu-id="5469c-119">Name</span></span>|<span data-ttu-id="5469c-120">说明</span><span class="sxs-lookup"><span data-stu-id="5469c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5469c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5469c-121">Authorization</span></span>|<span data-ttu-id="5469c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5469c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5469c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5469c-124">Content-Type</span></span>|<span data-ttu-id="5469c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5469c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5469c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5469c-127">Request body</span></span>

<span data-ttu-id="5469c-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5469c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5469c-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="5469c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5469c-130">参数</span><span class="sxs-lookup"><span data-stu-id="5469c-130">Parameter</span></span>|<span data-ttu-id="5469c-131">类型</span><span class="sxs-lookup"><span data-stu-id="5469c-131">Type</span></span>|<span data-ttu-id="5469c-132">说明</span><span class="sxs-lookup"><span data-stu-id="5469c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5469c-133">newAssignmentOrder</span><span class="sxs-lookup"><span data-stu-id="5469c-133">newAssignmentOrder</span></span>|[<span data-ttu-id="5469c-134">assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="5469c-134">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="5469c-135">用于定义在用户流中收集的属性的顺序。</span><span class="sxs-lookup"><span data-stu-id="5469c-135">Used to define the order of the attributes being collected within a user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="5469c-136">响应</span><span class="sxs-lookup"><span data-stu-id="5469c-136">Response</span></span>

<span data-ttu-id="5469c-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5469c-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5469c-138">示例</span><span class="sxs-lookup"><span data-stu-id="5469c-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5469c-139">请求</span><span class="sxs-lookup"><span data-stu-id="5469c-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "identityuserflowattributeassignment_setorder"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/userAttributeAssignments/setOrder
Content-Type: application/json
Content-length: 90

{
  "newAssignmentOrder": {
    "order": [
        "City",
        "extension_GUID_ShoeSize"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="5469c-140">响应</span><span class="sxs-lookup"><span data-stu-id="5469c-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
