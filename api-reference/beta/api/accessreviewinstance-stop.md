---
title: 停止访问ReviewInstance
description: 停止当前处于活动状态的 accessReviewInstance。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0655b0acd7dbd32b0ae4aae5337422f26f9c7c96
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048391"
---
# <a name="stop-accessreviewinstance"></a><span data-ttu-id="771fd-103">停止访问ReviewInstance</span><span class="sxs-lookup"><span data-stu-id="771fd-103">Stop accessReviewInstance</span></span>

<span data-ttu-id="771fd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="771fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="771fd-105">停止当前处于活动状态 [的 accessReviewInstance](../resources/accessreviewinstance.md)。</span><span class="sxs-lookup"><span data-stu-id="771fd-105">Stop a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="771fd-106">若要阻止定期访问评审启动将来的实例，请更新该检查[](accessreviewscheduledefinition-update.md)以更改其计划的结束日期。</span><span class="sxs-lookup"><span data-stu-id="771fd-106">To prevent a recurring access review from starting future instances, [update it](accessreviewscheduledefinition-update.md) to change its scheduled end date.</span></span>  <span data-ttu-id="771fd-107">在访问评审停止后，审阅者无法再提供输入，并且可以应用访问评审决策。</span><span class="sxs-lookup"><span data-stu-id="771fd-107">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="771fd-108">权限</span><span class="sxs-lookup"><span data-stu-id="771fd-108">Permissions</span></span>
<span data-ttu-id="771fd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="771fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="771fd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="771fd-111">Permission type</span></span>                        | <span data-ttu-id="771fd-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="771fd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="771fd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="771fd-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="771fd-114">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="771fd-114">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="771fd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="771fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="771fd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="771fd-116">Not supported.</span></span>|
|<span data-ttu-id="771fd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="771fd-117">Application</span></span>                            | <span data-ttu-id="771fd-118">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="771fd-118">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="771fd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="771fd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/stop
```

## <a name="request-headers"></a><span data-ttu-id="771fd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="771fd-120">Request headers</span></span>
<span data-ttu-id="771fd-121">无。</span><span class="sxs-lookup"><span data-stu-id="771fd-121">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="771fd-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="771fd-122">Request body</span></span>
<span data-ttu-id="771fd-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="771fd-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="771fd-124">响应</span><span class="sxs-lookup"><span data-stu-id="771fd-124">Response</span></span>
<span data-ttu-id="771fd-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="771fd-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="771fd-127">示例</span><span class="sxs-lookup"><span data-stu-id="771fd-127">Examples</span></span>
### <a name="request"></a><span data-ttu-id="771fd-128">请求</span><span class="sxs-lookup"><span data-stu-id="771fd-128">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="771fd-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="771fd-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReviewInstance"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d/instances/61a617dd-238f-4037-8fa5-d800e515f5bc/stop
```
# <a name="c"></a>[<span data-ttu-id="771fd-130">C#</span><span class="sxs-lookup"><span data-stu-id="771fd-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="771fd-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="771fd-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="771fd-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="771fd-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="771fd-133">Java</span><span class="sxs-lookup"><span data-stu-id="771fd-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/stop-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="771fd-134">响应</span><span class="sxs-lookup"><span data-stu-id="771fd-134">Response</span></span>
><span data-ttu-id="771fd-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="771fd-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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
