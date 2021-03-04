---
title: 删除 userAttributeAssignment
description: 删除 identityUserFlowAttributeAssignment 对象。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9c4e54cdc248e88833d50d89ef6051925d3391db
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435145"
---
# <a name="delete-userattributeassignment"></a><span data-ttu-id="d81e9-103">删除 userAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="d81e9-103">Delete userAttributeAssignment</span></span>

<span data-ttu-id="d81e9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d81e9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d81e9-105">删除 [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d81e9-105">Delete an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d81e9-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d81e9-106">Permissions</span></span>

<span data-ttu-id="d81e9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d81e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d81e9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d81e9-109">Permission type</span></span>|<span data-ttu-id="d81e9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d81e9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d81e9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d81e9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d81e9-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d81e9-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="d81e9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d81e9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d81e9-114">不支持</span><span class="sxs-lookup"><span data-stu-id="d81e9-114">Not supported</span></span>|
|<span data-ttu-id="d81e9-115">Application</span><span class="sxs-lookup"><span data-stu-id="d81e9-115">Application</span></span>|<span data-ttu-id="d81e9-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d81e9-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d81e9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d81e9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
DELETE /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d81e9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d81e9-118">Request headers</span></span>

|<span data-ttu-id="d81e9-119">名称</span><span class="sxs-lookup"><span data-stu-id="d81e9-119">Name</span></span>|<span data-ttu-id="d81e9-120">说明</span><span class="sxs-lookup"><span data-stu-id="d81e9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d81e9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d81e9-121">Authorization</span></span>|<span data-ttu-id="d81e9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d81e9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d81e9-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="d81e9-124">Request body</span></span>

<span data-ttu-id="d81e9-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d81e9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d81e9-126">响应</span><span class="sxs-lookup"><span data-stu-id="d81e9-126">Response</span></span>

<span data-ttu-id="d81e9-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d81e9-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d81e9-128">示例</span><span class="sxs-lookup"><span data-stu-id="d81e9-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d81e9-129">请求</span><span class="sxs-lookup"><span data-stu-id="d81e9-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d81e9-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d81e9-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userattributeassignments_from_b2cidentityuserflow"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="d81e9-131">C#</span><span class="sxs-lookup"><span data-stu-id="d81e9-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userattributeassignments-from-b2cidentityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d81e9-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d81e9-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userattributeassignments-from-b2cidentityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d81e9-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d81e9-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userattributeassignments-from-b2cidentityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d81e9-134">Java</span><span class="sxs-lookup"><span data-stu-id="d81e9-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-userattributeassignments-from-b2cidentityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d81e9-135">响应</span><span class="sxs-lookup"><span data-stu-id="d81e9-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
