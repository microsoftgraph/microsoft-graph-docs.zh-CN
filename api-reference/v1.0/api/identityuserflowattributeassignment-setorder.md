---
title: identityUserFlowAttributeAssignment：setOrder
description: 设置在用户流中收集的 identityUserFlowAttributeAssignments 的顺序。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: dc9e539b56d44bcfedf5818b7be6126421fedd96
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920641"
---
# <a name="identityuserflowattributeassignment-setorder"></a><span data-ttu-id="d82d5-103">identityUserFlowAttributeAssignment：setOrder</span><span class="sxs-lookup"><span data-stu-id="d82d5-103">identityUserFlowAttributeAssignment: setOrder</span></span>

<span data-ttu-id="d82d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d82d5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d82d5-105">设置在用户流中收集的 identityUserFlowAttributeAssignments 的顺序。</span><span class="sxs-lookup"><span data-stu-id="d82d5-105">Set the order of identityUserFlowAttributeAssignments being collected within a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="d82d5-106">权限</span><span class="sxs-lookup"><span data-stu-id="d82d5-106">Permissions</span></span>

<span data-ttu-id="d82d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d82d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d82d5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d82d5-109">Permission type</span></span>|<span data-ttu-id="d82d5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d82d5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d82d5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d82d5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d82d5-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d82d5-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="d82d5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d82d5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d82d5-114">不支持</span><span class="sxs-lookup"><span data-stu-id="d82d5-114">Not supported</span></span>|
|<span data-ttu-id="d82d5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d82d5-115">Application</span></span>|<span data-ttu-id="d82d5-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d82d5-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d82d5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d82d5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/setOrder
```

## <a name="request-headers"></a><span data-ttu-id="d82d5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d82d5-118">Request headers</span></span>

|<span data-ttu-id="d82d5-119">名称</span><span class="sxs-lookup"><span data-stu-id="d82d5-119">Name</span></span>|<span data-ttu-id="d82d5-120">说明</span><span class="sxs-lookup"><span data-stu-id="d82d5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d82d5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d82d5-121">Authorization</span></span>|<span data-ttu-id="d82d5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d82d5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d82d5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d82d5-124">Content-Type</span></span>|<span data-ttu-id="d82d5-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d82d5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d82d5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d82d5-127">Request body</span></span>

<span data-ttu-id="d82d5-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d82d5-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d82d5-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="d82d5-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d82d5-130">参数</span><span class="sxs-lookup"><span data-stu-id="d82d5-130">Parameter</span></span>|<span data-ttu-id="d82d5-131">类型</span><span class="sxs-lookup"><span data-stu-id="d82d5-131">Type</span></span>|<span data-ttu-id="d82d5-132">说明</span><span class="sxs-lookup"><span data-stu-id="d82d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d82d5-133">newAssignmentOrder</span><span class="sxs-lookup"><span data-stu-id="d82d5-133">newAssignmentOrder</span></span>|[<span data-ttu-id="d82d5-134">assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="d82d5-134">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="d82d5-135">用于定义在用户流中收集的属性的顺序。</span><span class="sxs-lookup"><span data-stu-id="d82d5-135">Used to define the order of the attributes being collected within a user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="d82d5-136">响应</span><span class="sxs-lookup"><span data-stu-id="d82d5-136">Response</span></span>

<span data-ttu-id="d82d5-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d82d5-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d82d5-138">示例</span><span class="sxs-lookup"><span data-stu-id="d82d5-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d82d5-139">请求</span><span class="sxs-lookup"><span data-stu-id="d82d5-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d82d5-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="d82d5-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d82d5-141">C#</span><span class="sxs-lookup"><span data-stu-id="d82d5-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityuserflowattributeassignment-setorder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d82d5-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d82d5-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityuserflowattributeassignment-setorder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d82d5-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d82d5-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityuserflowattributeassignment-setorder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d82d5-144">Java</span><span class="sxs-lookup"><span data-stu-id="d82d5-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityuserflowattributeassignment-setorder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d82d5-145">响应</span><span class="sxs-lookup"><span data-stu-id="d82d5-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
