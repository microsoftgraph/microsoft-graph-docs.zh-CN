---
title: 停止 accessReviewInstance
description: 停止当前处于活动状态的 accessReviewInstance。
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7e2ab7d5dddfbc1b5903f4a4379e8133278dc6bc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49221991"
---
# <a name="stop-accessreviewinstance"></a><span data-ttu-id="2f5c6-103">停止 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="2f5c6-103">Stop accessReviewInstance</span></span>

<span data-ttu-id="2f5c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f5c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f5c6-105">停止当前处于活动状态的 [accessReviewInstance](../resources/accessreviewinstance.md)。</span><span class="sxs-lookup"><span data-stu-id="2f5c6-105">Stop a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="2f5c6-106">若要防止定期访问审核启动以后的实例，请 [更新它](accessreviewscheduledefinition-update.md) 以更改计划的结束日期。</span><span class="sxs-lookup"><span data-stu-id="2f5c6-106">To prevent a recurring access review from starting future instances, [update it](accessreviewscheduledefinition-update.md) to change its scheduled end date.</span></span>  <span data-ttu-id="2f5c6-107">在访问审核停止后，审阅者无法再提供输入，并且可以应用访问审核决定。</span><span class="sxs-lookup"><span data-stu-id="2f5c6-107">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="2f5c6-108">权限</span><span class="sxs-lookup"><span data-stu-id="2f5c6-108">Permissions</span></span>
<span data-ttu-id="2f5c6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f5c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f5c6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f5c6-111">Permission type</span></span>                        | <span data-ttu-id="2f5c6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f5c6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f5c6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f5c6-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f5c6-114">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f5c6-114">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="2f5c6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f5c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f5c6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f5c6-116">Not supported.</span></span>|
|<span data-ttu-id="2f5c6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f5c6-117">Application</span></span>                            | <span data-ttu-id="2f5c6-118">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f5c6-118">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f5c6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f5c6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/stop
```

## <a name="request-headers"></a><span data-ttu-id="2f5c6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f5c6-120">Request headers</span></span>
<span data-ttu-id="2f5c6-121">无。</span><span class="sxs-lookup"><span data-stu-id="2f5c6-121">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="2f5c6-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f5c6-122">Request body</span></span>
<span data-ttu-id="2f5c6-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2f5c6-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f5c6-124">响应</span><span class="sxs-lookup"><span data-stu-id="2f5c6-124">Response</span></span>
<span data-ttu-id="2f5c6-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2f5c6-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f5c6-127">示例</span><span class="sxs-lookup"><span data-stu-id="2f5c6-127">Examples</span></span>
### <a name="request"></a><span data-ttu-id="2f5c6-128">请求</span><span class="sxs-lookup"><span data-stu-id="2f5c6-128">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2f5c6-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f5c6-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReviewInstance"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d/instances/61a617dd-238f-4037-8fa5-d800e515f5bc/stop
```
# <a name="c"></a>[<span data-ttu-id="2f5c6-130">C#</span><span class="sxs-lookup"><span data-stu-id="2f5c6-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f5c6-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f5c6-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f5c6-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f5c6-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f5c6-133">Java</span><span class="sxs-lookup"><span data-stu-id="2f5c6-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/stop-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="2f5c6-134">响应</span><span class="sxs-lookup"><span data-stu-id="2f5c6-134">Response</span></span>
><span data-ttu-id="2f5c6-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2f5c6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
