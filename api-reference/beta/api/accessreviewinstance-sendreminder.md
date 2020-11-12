---
title: 'accessReviewInstance: sendReminder'
description: 将提醒发送给当前活动的 accessReviewInstance 的审阅者。
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a31cf197cd8df1f806d5c9ead2b57903d632f1dc
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000815"
---
# <a name="accessreviewinstance-sendreminder"></a><span data-ttu-id="96d65-103">accessReviewInstance: sendReminder</span><span class="sxs-lookup"><span data-stu-id="96d65-103">accessReviewInstance: sendReminder</span></span>

<span data-ttu-id="96d65-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96d65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96d65-105">向当前活动的 [accessReviewInstance](../resources/accessreviewinstance.md)的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="96d65-105">Send a reminder to the reviewers of a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="96d65-106">权限</span><span class="sxs-lookup"><span data-stu-id="96d65-106">Permissions</span></span>
<span data-ttu-id="96d65-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96d65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96d65-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="96d65-109">Permission type</span></span>                        | <span data-ttu-id="96d65-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96d65-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="96d65-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96d65-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="96d65-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96d65-112">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="96d65-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96d65-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96d65-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="96d65-114">Not supported.</span></span>|
|<span data-ttu-id="96d65-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="96d65-115">Application</span></span>                            | <span data-ttu-id="96d65-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96d65-116">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="96d65-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96d65-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definitionId}/instances/{instanceId}/sendReminder
```
## <a name="request-headers"></a><span data-ttu-id="96d65-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="96d65-118">Request headers</span></span>
<span data-ttu-id="96d65-119">无。</span><span class="sxs-lookup"><span data-stu-id="96d65-119">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="96d65-120">请求正文</span><span class="sxs-lookup"><span data-stu-id="96d65-120">Request body</span></span>
<span data-ttu-id="96d65-121">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96d65-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96d65-122">响应</span><span class="sxs-lookup"><span data-stu-id="96d65-122">Response</span></span>
<span data-ttu-id="96d65-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="96d65-p102">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="96d65-125">示例</span><span class="sxs-lookup"><span data-stu-id="96d65-125">Examples</span></span>
### <a name="request"></a><span data-ttu-id="96d65-126">请求</span><span class="sxs-lookup"><span data-stu-id="96d65-126">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/04e5c3b2-9db2-40d3-a204-128f4956ae8e/instances/70463350-742e-4909-bfa5-bc23447bd002/sendReminder
```

---

### <a name="response"></a><span data-ttu-id="96d65-127">响应</span><span class="sxs-lookup"><span data-stu-id="96d65-127">Response</span></span>
><span data-ttu-id="96d65-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="96d65-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
