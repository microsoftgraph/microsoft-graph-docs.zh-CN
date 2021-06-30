---
title: accessReviewInstance：resetDecisions
description: 将 accessReviewInstance 上的所有 accessReviewInstanceDecisionItem 对象重置为 `notReviewed` 。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: df7e05103434c7b036d912ccdf8cd9ef6367b90f
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207510"
---
# <a name="accessreviewinstance-resetdecisions"></a><span data-ttu-id="9f4c5-103">accessReviewInstance：resetDecisions</span><span class="sxs-lookup"><span data-stu-id="9f4c5-103">accessReviewInstance: resetDecisions</span></span>
<span data-ttu-id="9f4c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f4c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f4c5-105">将 [accessReviewInstance 上的所有 accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象 [的决策](../resources/accessreviewinstance.md) 重置为 `notReviewed` 。</span><span class="sxs-lookup"><span data-stu-id="9f4c5-105">Resets decisions of all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects on an [accessReviewInstance](../resources/accessreviewinstance.md) to `notReviewed`.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f4c5-106">权限</span><span class="sxs-lookup"><span data-stu-id="9f4c5-106">Permissions</span></span>
<span data-ttu-id="9f4c5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f4c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f4c5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f4c5-109">Permission type</span></span>|<span data-ttu-id="9f4c5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9f4c5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f4c5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f4c5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9f4c5-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f4c5-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="9f4c5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f4c5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f4c5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f4c5-114">Not supported.</span></span>|
|<span data-ttu-id="9f4c5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f4c5-115">Application</span></span>|<span data-ttu-id="9f4c5-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f4c5-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f4c5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f4c5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/resetDecisions
```

## <a name="request-headers"></a><span data-ttu-id="9f4c5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f4c5-118">Request headers</span></span>
|<span data-ttu-id="9f4c5-119">名称</span><span class="sxs-lookup"><span data-stu-id="9f4c5-119">Name</span></span>|<span data-ttu-id="9f4c5-120">说明</span><span class="sxs-lookup"><span data-stu-id="9f4c5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9f4c5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f4c5-121">Authorization</span></span>|<span data-ttu-id="9f4c5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9f4c5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f4c5-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f4c5-124">Request body</span></span>
<span data-ttu-id="9f4c5-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9f4c5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f4c5-126">响应</span><span class="sxs-lookup"><span data-stu-id="9f4c5-126">Response</span></span>

<span data-ttu-id="9f4c5-127">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9f4c5-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9f4c5-128">示例</span><span class="sxs-lookup"><span data-stu-id="9f4c5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9f4c5-129">请求</span><span class="sxs-lookup"><span data-stu-id="9f4c5-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9f4c5-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f4c5-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_resetdecisions"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/0185aab8-9a7e-44b5-ae36-41b923c3bf87/instances/1234aab8-9a7e-44b5-ae36-41b923c3bf87/resetDecisions
```
# <a name="c"></a>[<span data-ttu-id="9f4c5-131">C#</span><span class="sxs-lookup"><span data-stu-id="9f4c5-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-resetdecisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f4c5-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f4c5-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-resetdecisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f4c5-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f4c5-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-resetdecisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9f4c5-134">Java</span><span class="sxs-lookup"><span data-stu-id="9f4c5-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-resetdecisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9f4c5-135">响应</span><span class="sxs-lookup"><span data-stu-id="9f4c5-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
