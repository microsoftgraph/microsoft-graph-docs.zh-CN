---
title: accessReviewInstance：resetDecisions
description: 将 accessReviewInstance 上的所有 accessReviewInstanceDecisionItem 对象重置为 `notReviewed` 。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: cfe9e5c0fe7390a9c2204678b7a926ef225154cf
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031442"
---
# <a name="accessreviewinstance-resetdecisions"></a><span data-ttu-id="4dd02-103">accessReviewInstance：resetDecisions</span><span class="sxs-lookup"><span data-stu-id="4dd02-103">accessReviewInstance: resetDecisions</span></span>
<span data-ttu-id="4dd02-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dd02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4dd02-105">将 [accessReviewInstance 上的所有 accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象 [的决策](../resources/accessreviewinstance.md) 重置为 `notReviewed` 。</span><span class="sxs-lookup"><span data-stu-id="4dd02-105">Resets decisions of all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects on an [accessReviewInstance](../resources/accessreviewinstance.md) to `notReviewed`.</span></span>

## <a name="permissions"></a><span data-ttu-id="4dd02-106">权限</span><span class="sxs-lookup"><span data-stu-id="4dd02-106">Permissions</span></span>
<span data-ttu-id="4dd02-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4dd02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dd02-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4dd02-109">Permission type</span></span>|<span data-ttu-id="4dd02-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4dd02-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dd02-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4dd02-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4dd02-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dd02-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="4dd02-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4dd02-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dd02-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4dd02-114">Not supported.</span></span>|
|<span data-ttu-id="4dd02-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4dd02-115">Application</span></span>|<span data-ttu-id="4dd02-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dd02-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dd02-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4dd02-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/resetDecisions
```

## <a name="request-headers"></a><span data-ttu-id="4dd02-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4dd02-118">Request headers</span></span>
|<span data-ttu-id="4dd02-119">名称</span><span class="sxs-lookup"><span data-stu-id="4dd02-119">Name</span></span>|<span data-ttu-id="4dd02-120">说明</span><span class="sxs-lookup"><span data-stu-id="4dd02-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4dd02-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4dd02-121">Authorization</span></span>|<span data-ttu-id="4dd02-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4dd02-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dd02-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="4dd02-124">Request body</span></span>
<span data-ttu-id="4dd02-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4dd02-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4dd02-126">响应</span><span class="sxs-lookup"><span data-stu-id="4dd02-126">Response</span></span>

<span data-ttu-id="4dd02-127">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4dd02-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4dd02-128">示例</span><span class="sxs-lookup"><span data-stu-id="4dd02-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4dd02-129">请求</span><span class="sxs-lookup"><span data-stu-id="4dd02-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_resetdecisions"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/0185aab8-9a7e-44b5-ae36-41b923c3bf87/instances/1234aab8-9a7e-44b5-ae36-41b923c3bf87/resetDecisions
```


### <a name="response"></a><span data-ttu-id="4dd02-130">响应</span><span class="sxs-lookup"><span data-stu-id="4dd02-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
