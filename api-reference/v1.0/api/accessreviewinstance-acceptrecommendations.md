---
title: accessReviewInstance：acceptRecommendations
description: 允许接受有关访问评审实例的决策的建议，该实例尚未由作为审阅者的调用用户审阅。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 60a9e59579f094e2c517c33ee96276220062599b
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031082"
---
# <a name="accessreviewinstance-acceptrecommendations"></a><span data-ttu-id="8e8c7-103">accessReviewInstance：acceptRecommendations</span><span class="sxs-lookup"><span data-stu-id="8e8c7-103">accessReviewInstance: acceptRecommendations</span></span>

<span data-ttu-id="8e8c7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e8c7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e8c7-105">允许接受对调用用户是其审阅者的[accessReviewInstance](../resources/accessreviewinstance.md)对象上尚未审阅的所有[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)对象的建议。</span><span class="sxs-lookup"><span data-stu-id="8e8c7-105">Allows the acceptance of recommendations on all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects that have not been reviewed on an [accessReviewInstance](../resources/accessreviewinstance.md) object for which the calling user is a reviewer.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e8c7-106">权限</span><span class="sxs-lookup"><span data-stu-id="8e8c7-106">Permissions</span></span>
<span data-ttu-id="8e8c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e8c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e8c7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e8c7-109">Permission type</span></span>|<span data-ttu-id="8e8c7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e8c7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e8c7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e8c7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8e8c7-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e8c7-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="8e8c7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e8c7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e8c7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e8c7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e8c7-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e8c7-115">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/acceptRecommendations
```

## <a name="request-headers"></a><span data-ttu-id="8e8c7-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e8c7-116">Request headers</span></span>
|<span data-ttu-id="8e8c7-117">名称</span><span class="sxs-lookup"><span data-stu-id="8e8c7-117">Name</span></span>|<span data-ttu-id="8e8c7-118">说明</span><span class="sxs-lookup"><span data-stu-id="8e8c7-118">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8e8c7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e8c7-119">Authorization</span></span>|<span data-ttu-id="8e8c7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8e8c7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e8c7-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e8c7-122">Request body</span></span>
<span data-ttu-id="8e8c7-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8e8c7-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e8c7-124">响应</span><span class="sxs-lookup"><span data-stu-id="8e8c7-124">Response</span></span>

<span data-ttu-id="8e8c7-125">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8e8c7-125">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8e8c7-126">示例</span><span class="sxs-lookup"><span data-stu-id="8e8c7-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8e8c7-127">请求</span><span class="sxs-lookup"><span data-stu-id="8e8c7-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_acceptrecommendations"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/1234fba0-cbf0-5678-8868-0810c7f91006/acceptRecommendations
```


### <a name="response"></a><span data-ttu-id="8e8c7-128">响应</span><span class="sxs-lookup"><span data-stu-id="8e8c7-128">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
