---
title: 删除 userAttributeAssignment
description: 删除 identityUserFlowAttributeAssignment 对象。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c7b83e264c05c3636f21237529c85b567a5eea8d
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689543"
---
# <a name="delete-userattributeassignment"></a><span data-ttu-id="7a2ba-103">删除 userAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="7a2ba-103">Delete userAttributeAssignment</span></span>

<span data-ttu-id="7a2ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a2ba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7a2ba-105">删除 [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7a2ba-105">Delete an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a2ba-106">权限</span><span class="sxs-lookup"><span data-stu-id="7a2ba-106">Permissions</span></span>

<span data-ttu-id="7a2ba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a2ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a2ba-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a2ba-109">Permission type</span></span>|<span data-ttu-id="7a2ba-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7a2ba-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a2ba-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a2ba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7a2ba-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a2ba-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="7a2ba-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a2ba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a2ba-114">不支持</span><span class="sxs-lookup"><span data-stu-id="7a2ba-114">Not supported</span></span>|
|<span data-ttu-id="7a2ba-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a2ba-115">Application</span></span>|<span data-ttu-id="7a2ba-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a2ba-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a2ba-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a2ba-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
DELETE /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7a2ba-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a2ba-118">Request headers</span></span>

|<span data-ttu-id="7a2ba-119">名称</span><span class="sxs-lookup"><span data-stu-id="7a2ba-119">Name</span></span>|<span data-ttu-id="7a2ba-120">说明</span><span class="sxs-lookup"><span data-stu-id="7a2ba-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7a2ba-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a2ba-121">Authorization</span></span>|<span data-ttu-id="7a2ba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7a2ba-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a2ba-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a2ba-124">Request body</span></span>

<span data-ttu-id="7a2ba-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7a2ba-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a2ba-126">响应</span><span class="sxs-lookup"><span data-stu-id="7a2ba-126">Response</span></span>

<span data-ttu-id="7a2ba-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7a2ba-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7a2ba-128">示例</span><span class="sxs-lookup"><span data-stu-id="7a2ba-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7a2ba-129">请求</span><span class="sxs-lookup"><span data-stu-id="7a2ba-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7a2ba-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a2ba-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userattributeassignments_from_b2cidentityuserflow"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="7a2ba-131">C#</span><span class="sxs-lookup"><span data-stu-id="7a2ba-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userattributeassignments-from-b2cidentityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a2ba-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a2ba-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userattributeassignments-from-b2cidentityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a2ba-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a2ba-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userattributeassignments-from-b2cidentityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a2ba-134">Java</span><span class="sxs-lookup"><span data-stu-id="7a2ba-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-userattributeassignments-from-b2cidentityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7a2ba-135">响应</span><span class="sxs-lookup"><span data-stu-id="7a2ba-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
