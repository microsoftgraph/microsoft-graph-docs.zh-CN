---
title: accessReviewInstance：resetDecisions
description: 将 accessReviewInstance 上的所有 accessReviewInstanceDecisionItem 对象重置为 `notReviewed` 。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 269c3f4891fb62d9191991ffa50dc70635268020
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209760"
---
# <a name="accessreviewinstance-resetdecisions"></a><span data-ttu-id="69f80-103">accessReviewInstance：resetDecisions</span><span class="sxs-lookup"><span data-stu-id="69f80-103">accessReviewInstance: resetDecisions</span></span>
<span data-ttu-id="69f80-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69f80-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69f80-105">将[accessReviewInstance 上的所有 accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)对象重置为[](../resources/accessreviewinstance.md) `notReviewed` 。</span><span class="sxs-lookup"><span data-stu-id="69f80-105">Resets all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects on an [accessReviewInstance](../resources/accessreviewinstance.md) to `notReviewed`.</span></span>

## <a name="permissions"></a><span data-ttu-id="69f80-106">权限</span><span class="sxs-lookup"><span data-stu-id="69f80-106">Permissions</span></span>
<span data-ttu-id="69f80-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69f80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69f80-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="69f80-109">Permission type</span></span>|<span data-ttu-id="69f80-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69f80-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69f80-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69f80-111">Delegated (work or school account)</span></span>|<span data-ttu-id="69f80-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f80-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="69f80-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69f80-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69f80-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="69f80-114">Not supported.</span></span>|
|<span data-ttu-id="69f80-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="69f80-115">Application</span></span>|<span data-ttu-id="69f80-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f80-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69f80-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69f80-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/resetDecisions
```

## <a name="request-headers"></a><span data-ttu-id="69f80-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="69f80-118">Request headers</span></span>
|<span data-ttu-id="69f80-119">名称</span><span class="sxs-lookup"><span data-stu-id="69f80-119">Name</span></span>|<span data-ttu-id="69f80-120">说明</span><span class="sxs-lookup"><span data-stu-id="69f80-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="69f80-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="69f80-121">Authorization</span></span>|<span data-ttu-id="69f80-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="69f80-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69f80-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="69f80-124">Request body</span></span>
<span data-ttu-id="69f80-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="69f80-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69f80-126">响应</span><span class="sxs-lookup"><span data-stu-id="69f80-126">Response</span></span>

<span data-ttu-id="69f80-127">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="69f80-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="69f80-128">示例</span><span class="sxs-lookup"><span data-stu-id="69f80-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="69f80-129">请求</span><span class="sxs-lookup"><span data-stu-id="69f80-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="69f80-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="69f80-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_resetdecisions"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances/1234a649-4f67-1234-88e7-55def6530e88/resetDecisions
```
# <a name="c"></a>[<span data-ttu-id="69f80-131">C#</span><span class="sxs-lookup"><span data-stu-id="69f80-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-resetdecisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69f80-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69f80-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-resetdecisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69f80-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69f80-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-resetdecisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="69f80-134">Java</span><span class="sxs-lookup"><span data-stu-id="69f80-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-resetdecisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="69f80-135">响应</span><span class="sxs-lookup"><span data-stu-id="69f80-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
