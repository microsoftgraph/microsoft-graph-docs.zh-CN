---
title: accessReviewInstance：sendReminder
description: 向当前处于活动状态的 accessReviewInstance 的审阅者发送提醒。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 00608ba03cbf3106b9707fc0e236328f2dfd1e65
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210957"
---
# <a name="accessreviewinstance-sendreminder"></a><span data-ttu-id="2e0c1-103">accessReviewInstance：sendReminder</span><span class="sxs-lookup"><span data-stu-id="2e0c1-103">accessReviewInstance: sendReminder</span></span>
<span data-ttu-id="2e0c1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e0c1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2e0c1-105">向活动 [accessReviewInstance](../resources/accessreviewinstance.md)的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="2e0c1-105">Send a reminder to the reviewers of an active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2e0c1-106">权限</span><span class="sxs-lookup"><span data-stu-id="2e0c1-106">Permissions</span></span>
<span data-ttu-id="2e0c1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e0c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e0c1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e0c1-109">Permission type</span></span>|<span data-ttu-id="2e0c1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2e0c1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e0c1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e0c1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2e0c1-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e0c1-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="2e0c1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e0c1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e0c1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e0c1-114">Not supported.</span></span>|
|<span data-ttu-id="2e0c1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e0c1-115">Application</span></span>|<span data-ttu-id="2e0c1-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e0c1-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e0c1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e0c1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/sendReminder
```

## <a name="request-headers"></a><span data-ttu-id="2e0c1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e0c1-118">Request headers</span></span>
|<span data-ttu-id="2e0c1-119">名称</span><span class="sxs-lookup"><span data-stu-id="2e0c1-119">Name</span></span>|<span data-ttu-id="2e0c1-120">说明</span><span class="sxs-lookup"><span data-stu-id="2e0c1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2e0c1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e0c1-121">Authorization</span></span>|<span data-ttu-id="2e0c1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2e0c1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e0c1-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e0c1-124">Request body</span></span>
<span data-ttu-id="2e0c1-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2e0c1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e0c1-126">响应</span><span class="sxs-lookup"><span data-stu-id="2e0c1-126">Response</span></span>

<span data-ttu-id="2e0c1-127">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2e0c1-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2e0c1-128">示例</span><span class="sxs-lookup"><span data-stu-id="2e0c1-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2e0c1-129">请求</span><span class="sxs-lookup"><span data-stu-id="2e0c1-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2e0c1-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e0c1-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_sendreminder"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances/1234a649-4f67-1234-88e7-55def6530e88/sendReminder
```
# <a name="c"></a>[<span data-ttu-id="2e0c1-131">C#</span><span class="sxs-lookup"><span data-stu-id="2e0c1-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-sendreminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e0c1-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e0c1-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-sendreminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e0c1-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e0c1-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-sendreminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e0c1-134">Java</span><span class="sxs-lookup"><span data-stu-id="2e0c1-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-sendreminder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2e0c1-135">响应</span><span class="sxs-lookup"><span data-stu-id="2e0c1-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
