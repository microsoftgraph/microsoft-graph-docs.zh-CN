---
title: accessReviewInstance：resetDecisions
description: 将 accessReviewInstance 上的所有 accessReviewInstanceDecisionItem 对象重置为 `notReviewed` 。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 778618535bc8d9d0eaf6dcc19ad697fa23de7db5
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031064"
---
# <a name="accessreviewinstance-resetdecisions"></a><span data-ttu-id="e83fc-103">accessReviewInstance：resetDecisions</span><span class="sxs-lookup"><span data-stu-id="e83fc-103">accessReviewInstance: resetDecisions</span></span>
<span data-ttu-id="e83fc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e83fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e83fc-105">将[accessReviewInstance 上的所有 accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)对象重置为[](../resources/accessreviewinstance.md) `notReviewed` 。</span><span class="sxs-lookup"><span data-stu-id="e83fc-105">Resets all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects on an [accessReviewInstance](../resources/accessreviewinstance.md) to `notReviewed`.</span></span>

## <a name="permissions"></a><span data-ttu-id="e83fc-106">权限</span><span class="sxs-lookup"><span data-stu-id="e83fc-106">Permissions</span></span>
<span data-ttu-id="e83fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e83fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e83fc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e83fc-109">Permission type</span></span>|<span data-ttu-id="e83fc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e83fc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e83fc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e83fc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e83fc-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e83fc-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="e83fc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e83fc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e83fc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e83fc-114">Not supported.</span></span>|
|<span data-ttu-id="e83fc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e83fc-115">Application</span></span>|<span data-ttu-id="e83fc-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e83fc-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e83fc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e83fc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/resetDecisions
```

## <a name="request-headers"></a><span data-ttu-id="e83fc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e83fc-118">Request headers</span></span>
|<span data-ttu-id="e83fc-119">名称</span><span class="sxs-lookup"><span data-stu-id="e83fc-119">Name</span></span>|<span data-ttu-id="e83fc-120">说明</span><span class="sxs-lookup"><span data-stu-id="e83fc-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e83fc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e83fc-121">Authorization</span></span>|<span data-ttu-id="e83fc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e83fc-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e83fc-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e83fc-124">Request body</span></span>
<span data-ttu-id="e83fc-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e83fc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e83fc-126">响应</span><span class="sxs-lookup"><span data-stu-id="e83fc-126">Response</span></span>

<span data-ttu-id="e83fc-127">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e83fc-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e83fc-128">示例</span><span class="sxs-lookup"><span data-stu-id="e83fc-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e83fc-129">请求</span><span class="sxs-lookup"><span data-stu-id="e83fc-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_resetdecisions"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances/1234a649-4f67-1234-88e7-55def6530e88/resetDecisions
```


### <a name="response"></a><span data-ttu-id="e83fc-130">响应</span><span class="sxs-lookup"><span data-stu-id="e83fc-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
