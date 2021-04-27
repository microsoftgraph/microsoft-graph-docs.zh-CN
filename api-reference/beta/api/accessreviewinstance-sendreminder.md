---
title: accessReviewInstance：sendReminder
description: 向当前处于活动状态的 accessReviewInstance 的审阅者发送提醒。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 20e662e0501091b4482c44450f4223ed5d39a95a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048405"
---
# <a name="accessreviewinstance-sendreminder"></a><span data-ttu-id="d60ee-103">accessReviewInstance：sendReminder</span><span class="sxs-lookup"><span data-stu-id="d60ee-103">accessReviewInstance: sendReminder</span></span>

<span data-ttu-id="d60ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d60ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d60ee-105">向当前处于活动状态的 [accessReviewInstance](../resources/accessreviewinstance.md)的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="d60ee-105">Send a reminder to the reviewers of a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d60ee-106">权限</span><span class="sxs-lookup"><span data-stu-id="d60ee-106">Permissions</span></span>
<span data-ttu-id="d60ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d60ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d60ee-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d60ee-109">Permission type</span></span>                        | <span data-ttu-id="d60ee-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d60ee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d60ee-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d60ee-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d60ee-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d60ee-112">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="d60ee-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d60ee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d60ee-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d60ee-114">Not supported.</span></span>|
|<span data-ttu-id="d60ee-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d60ee-115">Application</span></span>                            | <span data-ttu-id="d60ee-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d60ee-116">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d60ee-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d60ee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definitionId}/instances/{instanceId}/sendReminder
```
## <a name="request-headers"></a><span data-ttu-id="d60ee-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d60ee-118">Request headers</span></span>
<span data-ttu-id="d60ee-119">无。</span><span class="sxs-lookup"><span data-stu-id="d60ee-119">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="d60ee-120">请求正文</span><span class="sxs-lookup"><span data-stu-id="d60ee-120">Request body</span></span>
<span data-ttu-id="d60ee-121">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d60ee-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d60ee-122">响应</span><span class="sxs-lookup"><span data-stu-id="d60ee-122">Response</span></span>
<span data-ttu-id="d60ee-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d60ee-p102">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d60ee-125">示例</span><span class="sxs-lookup"><span data-stu-id="d60ee-125">Examples</span></span>
### <a name="request"></a><span data-ttu-id="d60ee-126">请求</span><span class="sxs-lookup"><span data-stu-id="d60ee-126">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d60ee-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="d60ee-127">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview_2"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/04e5c3b2-9db2-40d3-a204-128f4956ae8e/instances/70463350-742e-4909-bfa5-bc23447bd002/sendReminder
```
# <a name="c"></a>[<span data-ttu-id="d60ee-128">C#</span><span class="sxs-lookup"><span data-stu-id="d60ee-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sendreminder-accessreview-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d60ee-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d60ee-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sendreminder-accessreview-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d60ee-130">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d60ee-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sendreminder-accessreview-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d60ee-131">Java</span><span class="sxs-lookup"><span data-stu-id="d60ee-131">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sendreminder-accessreview-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="d60ee-132">响应</span><span class="sxs-lookup"><span data-stu-id="d60ee-132">Response</span></span>
><span data-ttu-id="d60ee-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d60ee-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
