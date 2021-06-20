---
title: accessReviewInstance：sendReminder
description: 向当前处于活动状态的 accessReviewInstance 的审阅者发送提醒。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8e47c8cb68d1cba3d6933dd62d68d930deb6b0bb
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031063"
---
# <a name="accessreviewinstance-sendreminder"></a><span data-ttu-id="d6457-103">accessReviewInstance：sendReminder</span><span class="sxs-lookup"><span data-stu-id="d6457-103">accessReviewInstance: sendReminder</span></span>
<span data-ttu-id="d6457-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6457-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d6457-105">向活动 [accessReviewInstance](../resources/accessreviewinstance.md)的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="d6457-105">Send a reminder to the reviewers of an active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d6457-106">权限</span><span class="sxs-lookup"><span data-stu-id="d6457-106">Permissions</span></span>
<span data-ttu-id="d6457-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6457-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6457-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6457-109">Permission type</span></span>|<span data-ttu-id="d6457-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6457-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6457-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6457-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d6457-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6457-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="d6457-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6457-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6457-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6457-114">Not supported.</span></span>|
|<span data-ttu-id="d6457-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6457-115">Application</span></span>|<span data-ttu-id="d6457-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6457-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6457-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6457-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/sendReminder
```

## <a name="request-headers"></a><span data-ttu-id="d6457-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6457-118">Request headers</span></span>
|<span data-ttu-id="d6457-119">名称</span><span class="sxs-lookup"><span data-stu-id="d6457-119">Name</span></span>|<span data-ttu-id="d6457-120">说明</span><span class="sxs-lookup"><span data-stu-id="d6457-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d6457-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6457-121">Authorization</span></span>|<span data-ttu-id="d6457-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6457-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6457-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6457-124">Request body</span></span>
<span data-ttu-id="d6457-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d6457-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6457-126">响应</span><span class="sxs-lookup"><span data-stu-id="d6457-126">Response</span></span>

<span data-ttu-id="d6457-127">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d6457-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d6457-128">示例</span><span class="sxs-lookup"><span data-stu-id="d6457-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d6457-129">请求</span><span class="sxs-lookup"><span data-stu-id="d6457-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_sendreminder"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances/1234a649-4f67-1234-88e7-55def6530e88/sendReminder
```


### <a name="response"></a><span data-ttu-id="d6457-130">响应</span><span class="sxs-lookup"><span data-stu-id="d6457-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
