---
title: 停止访问ReviewInstance
description: 停止当前处于活动状态的 accessReviewInstance。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c59b08c3a451d54a03502b28d2f05350f38e126f
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030486"
---
# <a name="stop-accessreviewinstance"></a><span data-ttu-id="d1aa2-103">停止访问ReviewInstance</span><span class="sxs-lookup"><span data-stu-id="d1aa2-103">Stop accessReviewInstance</span></span>

<span data-ttu-id="d1aa2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1aa2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1aa2-105">停止当前处于活动状态 [的 accessReviewInstance](../resources/accessreviewinstance.md)。</span><span class="sxs-lookup"><span data-stu-id="d1aa2-105">Stop a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="d1aa2-106">访问评审实例停止后，实例状态将为 ，审阅者无法再提供输入，并且可以 `Completed` 应用访问评审决策。</span><span class="sxs-lookup"><span data-stu-id="d1aa2-106">After the access review instance stops, the instance status will be `Completed`, the reviewers can no longer give input, and the access review decisions can be applied.</span></span>

<span data-ttu-id="d1aa2-107">停止实例将影响未来的实例。</span><span class="sxs-lookup"><span data-stu-id="d1aa2-107">Stopping an instance will not effect future instances.</span></span> <span data-ttu-id="d1aa2-108">若要防止定期访问评审启动将来的实例，请 [更新计划定义](accessreviewscheduledefinition-update.md) 以更改其计划的结束日期。</span><span class="sxs-lookup"><span data-stu-id="d1aa2-108">To prevent a recurring access review from starting future instances, [update the schedule definition](accessreviewscheduledefinition-update.md) to change its scheduled end date.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1aa2-109">权限</span><span class="sxs-lookup"><span data-stu-id="d1aa2-109">Permissions</span></span>
<span data-ttu-id="d1aa2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1aa2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1aa2-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1aa2-112">Permission type</span></span>                        | <span data-ttu-id="d1aa2-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1aa2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1aa2-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1aa2-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1aa2-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1aa2-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="d1aa2-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1aa2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1aa2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1aa2-117">Not supported.</span></span>|
|<span data-ttu-id="d1aa2-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1aa2-118">Application</span></span>                            | <span data-ttu-id="d1aa2-119">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1aa2-119">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1aa2-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1aa2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/stop
```

## <a name="request-headers"></a><span data-ttu-id="d1aa2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1aa2-121">Request headers</span></span>
<span data-ttu-id="d1aa2-122">无。</span><span class="sxs-lookup"><span data-stu-id="d1aa2-122">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="d1aa2-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1aa2-123">Request body</span></span>
<span data-ttu-id="d1aa2-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d1aa2-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1aa2-125">响应</span><span class="sxs-lookup"><span data-stu-id="d1aa2-125">Response</span></span>
<span data-ttu-id="d1aa2-p104">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d1aa2-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1aa2-128">示例</span><span class="sxs-lookup"><span data-stu-id="d1aa2-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="d1aa2-129">请求</span><span class="sxs-lookup"><span data-stu-id="d1aa2-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d1aa2-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1aa2-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReviewInstance"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d/instances/61a617dd-238f-4037-8fa5-d800e515f5bc/stop
```
# <a name="c"></a>[<span data-ttu-id="d1aa2-131">C#</span><span class="sxs-lookup"><span data-stu-id="d1aa2-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1aa2-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1aa2-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1aa2-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1aa2-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1aa2-134">Java</span><span class="sxs-lookup"><span data-stu-id="d1aa2-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/stop-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="d1aa2-135">响应</span><span class="sxs-lookup"><span data-stu-id="d1aa2-135">Response</span></span>
><span data-ttu-id="d1aa2-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d1aa2-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Stop accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
