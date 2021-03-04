---
title: 删除 accessReviewScheduleDefinition
description: 删除 accessReviewScheduleDefinition 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9bf7197643ca0b445e11d59e97693c80a9627913
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439077"
---
# <a name="delete-accessreviewscheduledefinition"></a><span data-ttu-id="33102-103">删除 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="33102-103">Delete accessReviewScheduleDefinition</span></span>

<span data-ttu-id="33102-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33102-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33102-105">删除 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="33102-105">Delete an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="33102-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="33102-106">Permissions</span></span>
<span data-ttu-id="33102-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="33102-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33102-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="33102-109">Permission type</span></span>                        | <span data-ttu-id="33102-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="33102-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="33102-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="33102-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="33102-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33102-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="33102-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="33102-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33102-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="33102-114">Not supported.</span></span>|
|<span data-ttu-id="33102-115">Application</span><span class="sxs-lookup"><span data-stu-id="33102-115">Application</span></span>                            | <span data-ttu-id="33102-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33102-116">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33102-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="33102-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="33102-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="33102-118">Request headers</span></span>
<span data-ttu-id="33102-119">无。</span><span class="sxs-lookup"><span data-stu-id="33102-119">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="33102-120">请求正文</span><span class="sxs-lookup"><span data-stu-id="33102-120">Request body</span></span>
<span data-ttu-id="33102-121">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="33102-121">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="33102-122">响应</span><span class="sxs-lookup"><span data-stu-id="33102-122">Response</span></span>
<span data-ttu-id="33102-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="33102-p102">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="33102-125">示例</span><span class="sxs-lookup"><span data-stu-id="33102-125">Examples</span></span>
### <a name="request"></a><span data-ttu-id="33102-126">请求</span><span class="sxs-lookup"><span data-stu-id="33102-126">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="33102-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="33102-127">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accessReviewScheduleDefinition"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/29f2d16e-9ca6-4052-bbfe-802c48981fd8
```
# <a name="c"></a>[<span data-ttu-id="33102-128">C#</span><span class="sxs-lookup"><span data-stu-id="33102-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33102-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33102-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33102-130">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33102-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33102-131">Java</span><span class="sxs-lookup"><span data-stu-id="33102-131">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="33102-132">响应</span><span class="sxs-lookup"><span data-stu-id="33102-132">Response</span></span>
><span data-ttu-id="33102-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="33102-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
