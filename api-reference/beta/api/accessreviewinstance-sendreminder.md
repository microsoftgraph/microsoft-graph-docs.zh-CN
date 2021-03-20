---
title: accessReviewInstance：sendReminder
description: 向当前处于活动状态的 accessReviewInstance 的审阅者发送提醒。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8d18613b1fc59db04ce0f7fdfe6d3937542ed0dd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943059"
---
# <a name="accessreviewinstance-sendreminder"></a><span data-ttu-id="c32f7-103">accessReviewInstance：sendReminder</span><span class="sxs-lookup"><span data-stu-id="c32f7-103">accessReviewInstance: sendReminder</span></span>

<span data-ttu-id="c32f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c32f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c32f7-105">向当前处于活动状态的 [accessReviewInstance](../resources/accessreviewinstance.md)的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="c32f7-105">Send a reminder to the reviewers of a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c32f7-106">权限</span><span class="sxs-lookup"><span data-stu-id="c32f7-106">Permissions</span></span>
<span data-ttu-id="c32f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c32f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c32f7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c32f7-109">Permission type</span></span>                        | <span data-ttu-id="c32f7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c32f7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c32f7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c32f7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c32f7-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c32f7-112">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="c32f7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c32f7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c32f7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c32f7-114">Not supported.</span></span>|
|<span data-ttu-id="c32f7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c32f7-115">Application</span></span>                            | <span data-ttu-id="c32f7-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c32f7-116">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c32f7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c32f7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definitionId}/instances/{instanceId}/sendReminder
```
## <a name="request-headers"></a><span data-ttu-id="c32f7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c32f7-118">Request headers</span></span>
<span data-ttu-id="c32f7-119">无。</span><span class="sxs-lookup"><span data-stu-id="c32f7-119">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="c32f7-120">请求正文</span><span class="sxs-lookup"><span data-stu-id="c32f7-120">Request body</span></span>
<span data-ttu-id="c32f7-121">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c32f7-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c32f7-122">响应</span><span class="sxs-lookup"><span data-stu-id="c32f7-122">Response</span></span>
<span data-ttu-id="c32f7-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c32f7-p102">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c32f7-125">示例</span><span class="sxs-lookup"><span data-stu-id="c32f7-125">Examples</span></span>
### <a name="request"></a><span data-ttu-id="c32f7-126">请求</span><span class="sxs-lookup"><span data-stu-id="c32f7-126">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c32f7-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="c32f7-127">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview_2"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/04e5c3b2-9db2-40d3-a204-128f4956ae8e/instances/70463350-742e-4909-bfa5-bc23447bd002/sendReminder
```
# <a name="c"></a>[<span data-ttu-id="c32f7-128">C#</span><span class="sxs-lookup"><span data-stu-id="c32f7-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sendreminder-accessreview-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c32f7-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c32f7-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sendreminder-accessreview-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c32f7-130">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c32f7-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sendreminder-accessreview-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c32f7-131">Java</span><span class="sxs-lookup"><span data-stu-id="c32f7-131">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sendreminder-accessreview-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="c32f7-132">响应</span><span class="sxs-lookup"><span data-stu-id="c32f7-132">Response</span></span>
><span data-ttu-id="c32f7-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c32f7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "SendReminder accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
