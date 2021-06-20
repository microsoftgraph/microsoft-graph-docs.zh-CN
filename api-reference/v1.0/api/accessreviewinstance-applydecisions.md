---
title: accessReviewInstance：applyDecisions
description: 对 accessReviewInstance 应用决策。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 93cc4d2e4f5c42ebe47bed00caf227779b579df2
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030302"
---
# <a name="accessreviewinstance-applydecisions"></a><span data-ttu-id="27c38-103">accessReviewInstance：applyDecisions</span><span class="sxs-lookup"><span data-stu-id="27c38-103">accessReviewInstance: applyDecisions</span></span>
<span data-ttu-id="27c38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27c38-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="27c38-105">将审阅决策应用于 [accessReviewInstance 中审阅的资源](../resources/accessreviewinstance.md)。</span><span class="sxs-lookup"><span data-stu-id="27c38-105">Apply review decisions to the resource reviewed in an [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

<span data-ttu-id="27c38-106">如果 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)的 **settings** 参数的 **autoApplyDecisionsEnabled** 为 ，则自动应用决策 `true` 。</span><span class="sxs-lookup"><span data-stu-id="27c38-106">Decisions are applied automatically if the **autoApplyDecisionsEnabled** of the **settings** parameter of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) is `true`.</span></span>

## <a name="permissions"></a><span data-ttu-id="27c38-107">权限</span><span class="sxs-lookup"><span data-stu-id="27c38-107">Permissions</span></span>
<span data-ttu-id="27c38-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27c38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27c38-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="27c38-110">Permission type</span></span>|<span data-ttu-id="27c38-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="27c38-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27c38-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27c38-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27c38-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27c38-113">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="27c38-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27c38-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27c38-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="27c38-115">Not supported.</span></span>|
|<span data-ttu-id="27c38-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="27c38-116">Application</span></span>|<span data-ttu-id="27c38-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27c38-117">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27c38-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27c38-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/applyDecisions
```

## <a name="request-headers"></a><span data-ttu-id="27c38-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="27c38-119">Request headers</span></span>
|<span data-ttu-id="27c38-120">名称</span><span class="sxs-lookup"><span data-stu-id="27c38-120">Name</span></span>|<span data-ttu-id="27c38-121">说明</span><span class="sxs-lookup"><span data-stu-id="27c38-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="27c38-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="27c38-122">Authorization</span></span>|<span data-ttu-id="27c38-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="27c38-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27c38-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="27c38-125">Request body</span></span>
<span data-ttu-id="27c38-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="27c38-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27c38-127">响应</span><span class="sxs-lookup"><span data-stu-id="27c38-127">Response</span></span>

<span data-ttu-id="27c38-128">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="27c38-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="27c38-129">示例</span><span class="sxs-lookup"><span data-stu-id="27c38-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27c38-130">请求</span><span class="sxs-lookup"><span data-stu-id="27c38-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_applydecisions"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/1234fba0-cbf0-5678-8868-0810c7f49101/applyDecisions
```


### <a name="response"></a><span data-ttu-id="27c38-131">响应</span><span class="sxs-lookup"><span data-stu-id="27c38-131">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
