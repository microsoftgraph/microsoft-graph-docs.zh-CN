---
title: accessReviewInstance：acceptRecommendations
description: 允许接受有关访问评审实例的决策的建议，该实例尚未由作为审阅者的调用用户审阅。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d8548340af184f703e89fcfd8aeda469d81cb566
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208154"
---
# <a name="accessreviewinstance-acceptrecommendations"></a><span data-ttu-id="d5c67-103">accessReviewInstance：acceptRecommendations</span><span class="sxs-lookup"><span data-stu-id="d5c67-103">accessReviewInstance: acceptRecommendations</span></span>

<span data-ttu-id="d5c67-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5c67-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5c67-105">允许接受对调用用户是其审阅者的[accessReviewInstance](../resources/accessreviewinstance.md)对象上尚未审阅的所有[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)对象的建议。</span><span class="sxs-lookup"><span data-stu-id="d5c67-105">Allows the acceptance of recommendations on all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects that have not been reviewed on an [accessReviewInstance](../resources/accessreviewinstance.md) object for which the calling user is a reviewer.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5c67-106">权限</span><span class="sxs-lookup"><span data-stu-id="d5c67-106">Permissions</span></span>
<span data-ttu-id="d5c67-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5c67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5c67-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5c67-109">Permission type</span></span>|<span data-ttu-id="d5c67-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5c67-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5c67-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5c67-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d5c67-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5c67-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="d5c67-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5c67-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5c67-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5c67-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5c67-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5c67-115">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/acceptRecommendations
```

## <a name="request-headers"></a><span data-ttu-id="d5c67-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5c67-116">Request headers</span></span>
|<span data-ttu-id="d5c67-117">名称</span><span class="sxs-lookup"><span data-stu-id="d5c67-117">Name</span></span>|<span data-ttu-id="d5c67-118">说明</span><span class="sxs-lookup"><span data-stu-id="d5c67-118">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d5c67-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5c67-119">Authorization</span></span>|<span data-ttu-id="d5c67-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5c67-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5c67-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5c67-122">Request body</span></span>
<span data-ttu-id="d5c67-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5c67-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5c67-124">响应</span><span class="sxs-lookup"><span data-stu-id="d5c67-124">Response</span></span>

<span data-ttu-id="d5c67-125">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d5c67-125">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d5c67-126">示例</span><span class="sxs-lookup"><span data-stu-id="d5c67-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d5c67-127">请求</span><span class="sxs-lookup"><span data-stu-id="d5c67-127">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d5c67-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5c67-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_acceptrecommendations"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/1234fba0-cbf0-5678-8868-0810c7f91006/acceptRecommendations
```
# <a name="c"></a>[<span data-ttu-id="d5c67-129">C#</span><span class="sxs-lookup"><span data-stu-id="d5c67-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-acceptrecommendations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5c67-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5c67-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-acceptrecommendations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5c67-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5c67-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-acceptrecommendations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d5c67-132">Java</span><span class="sxs-lookup"><span data-stu-id="d5c67-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-acceptrecommendations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d5c67-133">响应</span><span class="sxs-lookup"><span data-stu-id="d5c67-133">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
