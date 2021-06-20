---
title: accessReviewInstance：stop
description: 停止当前处于活动状态的 accessReviewInstance。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e119d3c914a793bfc083722fb329bd18a72b46df
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031062"
---
# <a name="accessreviewinstance-stop"></a><span data-ttu-id="18ce3-103">accessReviewInstance：stop</span><span class="sxs-lookup"><span data-stu-id="18ce3-103">accessReviewInstance: stop</span></span>
<span data-ttu-id="18ce3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18ce3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18ce3-105">停止当前处于活动状态 [的 accessReviewInstance](../resources/accessreviewinstance.md)。</span><span class="sxs-lookup"><span data-stu-id="18ce3-105">Stop a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="18ce3-106">访问评审实例停止后，实例状态将标记为 ，审阅者无法再提供输入，并应用访问 `Completed` 评审决策。</span><span class="sxs-lookup"><span data-stu-id="18ce3-106">After the access review instance stops, the instance status is marked as `Completed`, the reviewers can no longer give input, and the access review decisions are applied.</span></span>

<span data-ttu-id="18ce3-107">停止实例不会停止以后的实例。</span><span class="sxs-lookup"><span data-stu-id="18ce3-107">Stopping an instance will not stop future instances.</span></span> <span data-ttu-id="18ce3-108">若要防止定期访问评审启动将来的实例，请 [更新计划定义](accessreviewscheduledefinition-update.md) 以更改其计划的结束日期。</span><span class="sxs-lookup"><span data-stu-id="18ce3-108">To prevent a recurring access review from starting future instances, [update the schedule definition](accessreviewscheduledefinition-update.md) to change its scheduled end date.</span></span>

## <a name="permissions"></a><span data-ttu-id="18ce3-109">权限</span><span class="sxs-lookup"><span data-stu-id="18ce3-109">Permissions</span></span>
<span data-ttu-id="18ce3-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18ce3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18ce3-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="18ce3-112">Permission type</span></span>|<span data-ttu-id="18ce3-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18ce3-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18ce3-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18ce3-114">Delegated (work or school account)</span></span>|<span data-ttu-id="18ce3-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18ce3-115">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="18ce3-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18ce3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18ce3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="18ce3-117">Not supported.</span></span>|
|<span data-ttu-id="18ce3-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="18ce3-118">Application</span></span>|<span data-ttu-id="18ce3-119">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18ce3-119">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18ce3-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18ce3-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stop
```

## <a name="request-headers"></a><span data-ttu-id="18ce3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="18ce3-121">Request headers</span></span>
|<span data-ttu-id="18ce3-122">名称</span><span class="sxs-lookup"><span data-stu-id="18ce3-122">Name</span></span>|<span data-ttu-id="18ce3-123">说明</span><span class="sxs-lookup"><span data-stu-id="18ce3-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="18ce3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="18ce3-124">Authorization</span></span>|<span data-ttu-id="18ce3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="18ce3-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="18ce3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="18ce3-127">Request body</span></span>
<span data-ttu-id="18ce3-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="18ce3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18ce3-129">响应</span><span class="sxs-lookup"><span data-stu-id="18ce3-129">Response</span></span>

<span data-ttu-id="18ce3-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="18ce3-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="18ce3-131">示例</span><span class="sxs-lookup"><span data-stu-id="18ce3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="18ce3-132">请求</span><span class="sxs-lookup"><span data-stu-id="18ce3-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_stop"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances/1234a649-4f67-1234-88e7-55def6530e88/stop
```


### <a name="response"></a><span data-ttu-id="18ce3-133">响应</span><span class="sxs-lookup"><span data-stu-id="18ce3-133">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
