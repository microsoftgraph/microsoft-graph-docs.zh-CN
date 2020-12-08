---
title: 'identityUserFlowAttributeAssignment: setOrder'
description: 设置在用户流中收集的 identityUserFlowAttributeAssignments 的顺序。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 705acf8e65d7d01c40d98860c6f5066121d23a81
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581329"
---
# <a name="identityuserflowattributeassignment-setorder"></a><span data-ttu-id="4ad96-103">identityUserFlowAttributeAssignment: setOrder</span><span class="sxs-lookup"><span data-stu-id="4ad96-103">identityUserFlowAttributeAssignment: setOrder</span></span>

<span data-ttu-id="4ad96-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ad96-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ad96-105">设置在用户流中收集的 identityUserFlowAttributeAssignments 的顺序。</span><span class="sxs-lookup"><span data-stu-id="4ad96-105">Set the order of identityUserFlowAttributeAssignments being collected within a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ad96-106">权限</span><span class="sxs-lookup"><span data-stu-id="4ad96-106">Permissions</span></span>

<span data-ttu-id="4ad96-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ad96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ad96-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ad96-109">Permission type</span></span>|<span data-ttu-id="4ad96-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ad96-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ad96-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ad96-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4ad96-112">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="4ad96-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="4ad96-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ad96-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ad96-114">不支持</span><span class="sxs-lookup"><span data-stu-id="4ad96-114">Not supported</span></span>|
|<span data-ttu-id="4ad96-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ad96-115">Application</span></span>|<span data-ttu-id="4ad96-116">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="4ad96-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ad96-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ad96-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/setOrder
POST /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/setOrder
```

## <a name="request-headers"></a><span data-ttu-id="4ad96-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ad96-118">Request headers</span></span>

|<span data-ttu-id="4ad96-119">名称</span><span class="sxs-lookup"><span data-stu-id="4ad96-119">Name</span></span>|<span data-ttu-id="4ad96-120">说明</span><span class="sxs-lookup"><span data-stu-id="4ad96-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4ad96-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ad96-121">Authorization</span></span>|<span data-ttu-id="4ad96-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ad96-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4ad96-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4ad96-124">Content-Type</span></span>|<span data-ttu-id="4ad96-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4ad96-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ad96-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ad96-127">Request body</span></span>

<span data-ttu-id="4ad96-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ad96-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4ad96-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="4ad96-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4ad96-130">参数</span><span class="sxs-lookup"><span data-stu-id="4ad96-130">Parameter</span></span>|<span data-ttu-id="4ad96-131">类型</span><span class="sxs-lookup"><span data-stu-id="4ad96-131">Type</span></span>|<span data-ttu-id="4ad96-132">Description</span><span class="sxs-lookup"><span data-stu-id="4ad96-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ad96-133">newAssignmentOrder</span><span class="sxs-lookup"><span data-stu-id="4ad96-133">newAssignmentOrder</span></span>|[<span data-ttu-id="4ad96-134">assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="4ad96-134">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="4ad96-135">用于定义在用户流中收集的属性的顺序。</span><span class="sxs-lookup"><span data-stu-id="4ad96-135">Used to define the order of the attributes being collected within a user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="4ad96-136">响应</span><span class="sxs-lookup"><span data-stu-id="4ad96-136">Response</span></span>

<span data-ttu-id="4ad96-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4ad96-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4ad96-138">示例</span><span class="sxs-lookup"><span data-stu-id="4ad96-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4ad96-139">请求</span><span class="sxs-lookup"><span data-stu-id="4ad96-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "identityuserflowattributeassignment_setorder"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/setOrder

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

### <a name="response"></a><span data-ttu-id="4ad96-140">响应</span><span class="sxs-lookup"><span data-stu-id="4ad96-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
