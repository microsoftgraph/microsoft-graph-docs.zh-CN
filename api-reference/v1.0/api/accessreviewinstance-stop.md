---
title: accessReviewInstance：stop
description: 停止当前处于活动状态的 accessReviewInstance。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 08b9974b1b496a3ff50048d72dbb65659758658e
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211031"
---
# <a name="accessreviewinstance-stop"></a><span data-ttu-id="aa0ca-103">accessReviewInstance：stop</span><span class="sxs-lookup"><span data-stu-id="aa0ca-103">accessReviewInstance: stop</span></span>
<span data-ttu-id="aa0ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa0ca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aa0ca-105">停止当前处于活动状态 [的 accessReviewInstance](../resources/accessreviewinstance.md)。</span><span class="sxs-lookup"><span data-stu-id="aa0ca-105">Stop a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="aa0ca-106">访问评审实例停止后，实例状态将标记为 ，审阅者无法再提供输入，并应用访问 `Completed` 评审决策。</span><span class="sxs-lookup"><span data-stu-id="aa0ca-106">After the access review instance stops, the instance status is marked as `Completed`, the reviewers can no longer give input, and the access review decisions are applied.</span></span>

<span data-ttu-id="aa0ca-107">停止实例不会停止以后的实例。</span><span class="sxs-lookup"><span data-stu-id="aa0ca-107">Stopping an instance will not stop future instances.</span></span> <span data-ttu-id="aa0ca-108">若要防止定期访问评审启动将来的实例，请 [更新计划定义](accessreviewscheduledefinition-update.md) 以更改其计划的结束日期。</span><span class="sxs-lookup"><span data-stu-id="aa0ca-108">To prevent a recurring access review from starting future instances, [update the schedule definition](accessreviewscheduledefinition-update.md) to change its scheduled end date.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa0ca-109">权限</span><span class="sxs-lookup"><span data-stu-id="aa0ca-109">Permissions</span></span>
<span data-ttu-id="aa0ca-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa0ca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa0ca-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa0ca-112">Permission type</span></span>|<span data-ttu-id="aa0ca-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa0ca-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa0ca-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa0ca-114">Delegated (work or school account)</span></span>|<span data-ttu-id="aa0ca-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa0ca-115">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="aa0ca-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa0ca-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa0ca-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa0ca-117">Not supported.</span></span>|
|<span data-ttu-id="aa0ca-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa0ca-118">Application</span></span>|<span data-ttu-id="aa0ca-119">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa0ca-119">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa0ca-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa0ca-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stop
```

## <a name="request-headers"></a><span data-ttu-id="aa0ca-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa0ca-121">Request headers</span></span>
|<span data-ttu-id="aa0ca-122">名称</span><span class="sxs-lookup"><span data-stu-id="aa0ca-122">Name</span></span>|<span data-ttu-id="aa0ca-123">说明</span><span class="sxs-lookup"><span data-stu-id="aa0ca-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="aa0ca-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa0ca-124">Authorization</span></span>|<span data-ttu-id="aa0ca-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa0ca-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa0ca-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa0ca-127">Request body</span></span>
<span data-ttu-id="aa0ca-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aa0ca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa0ca-129">响应</span><span class="sxs-lookup"><span data-stu-id="aa0ca-129">Response</span></span>

<span data-ttu-id="aa0ca-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="aa0ca-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="aa0ca-131">示例</span><span class="sxs-lookup"><span data-stu-id="aa0ca-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aa0ca-132">请求</span><span class="sxs-lookup"><span data-stu-id="aa0ca-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="aa0ca-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa0ca-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_stop"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances/1234a649-4f67-1234-88e7-55def6530e88/stop
```
# <a name="c"></a>[<span data-ttu-id="aa0ca-134">C#</span><span class="sxs-lookup"><span data-stu-id="aa0ca-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-stop-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa0ca-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa0ca-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-stop-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa0ca-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa0ca-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-stop-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa0ca-137">Java</span><span class="sxs-lookup"><span data-stu-id="aa0ca-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-stop-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="aa0ca-138">响应</span><span class="sxs-lookup"><span data-stu-id="aa0ca-138">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
