---
title: accessReviewInstance：acceptRecommendations
description: '允许接受针对调用用户是审阅者的访问评审实例未审阅的所有决策的建议。 '
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b955bc637c3f536ca5cb8a3e24ad65990296ab2e
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030752"
---
# <a name="accessreviewinstance-acceptrecommendations"></a><span data-ttu-id="d5c88-103">accessReviewInstance：acceptRecommendations</span><span class="sxs-lookup"><span data-stu-id="d5c88-103">accessReviewInstance: acceptRecommendations</span></span>

<span data-ttu-id="d5c88-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5c88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5c88-105">允许接受有关所有 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象的建议，这些对象尚未针对调用用户作为审阅者的 [accessReviewInstance](../resources/accessreviewinstance.md) 对象进行审阅。</span><span class="sxs-lookup"><span data-stu-id="d5c88-105">Allows the acceptance of recommendations on all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects that have not been reviewed for an [accessReviewInstance](../resources/accessreviewinstance.md) object for which the calling user is a reviewer.</span></span> <span data-ttu-id="d5c88-106">推荐 **在** `true` [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)对象上时生成 recommendationsEnabled。</span><span class="sxs-lookup"><span data-stu-id="d5c88-106">Recommendations are generated if **recommendationsEnabled** is `true` on the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span> <span data-ttu-id="d5c88-107">如果没有对 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象的建议，将不会记录任何决策。</span><span class="sxs-lookup"><span data-stu-id="d5c88-107">If there is not a recommendation on an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object no decision will be recorded.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5c88-108">权限</span><span class="sxs-lookup"><span data-stu-id="d5c88-108">Permissions</span></span>
<span data-ttu-id="d5c88-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5c88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5c88-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5c88-111">Permission type</span></span>                        | <span data-ttu-id="d5c88-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5c88-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5c88-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5c88-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5c88-114">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5c88-114">AccessReview.ReadWrite.All</span></span> |
| <span data-ttu-id="d5c88-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5c88-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d5c88-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5c88-116">Not supported.</span></span> |

<span data-ttu-id="d5c88-117">登录用户还必须是 accessReviewInstance 上的审阅者。</span><span class="sxs-lookup"><span data-stu-id="d5c88-117">The signed-in user must also be a reviewer on the accessReviewInstance.</span></span>

## <a name="http-request"></a><span data-ttu-id="d5c88-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5c88-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/pendingAccessReviewInstances/{instance-id}/acceptRecommendations
```
## <a name="request-headers"></a><span data-ttu-id="d5c88-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5c88-119">Request headers</span></span>
<span data-ttu-id="d5c88-120">无。</span><span class="sxs-lookup"><span data-stu-id="d5c88-120">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="d5c88-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5c88-121">Request body</span></span>
<span data-ttu-id="d5c88-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5c88-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5c88-123">响应</span><span class="sxs-lookup"><span data-stu-id="d5c88-123">Response</span></span>
<span data-ttu-id="d5c88-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d5c88-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d5c88-126">示例</span><span class="sxs-lookup"><span data-stu-id="d5c88-126">Examples</span></span>
### <a name="request"></a><span data-ttu-id="d5c88-127">请求</span><span class="sxs-lookup"><span data-stu-id="d5c88-127">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d5c88-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5c88-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "acceptrecommendations_accessReviewInstance"
}-->
```http
POST https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/acceptRecommendations
```
# <a name="c"></a>[<span data-ttu-id="d5c88-129">C#</span><span class="sxs-lookup"><span data-stu-id="d5c88-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/acceptrecommendations-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5c88-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5c88-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/acceptrecommendations-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5c88-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5c88-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/acceptrecommendations-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d5c88-132">Java</span><span class="sxs-lookup"><span data-stu-id="d5c88-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/acceptrecommendations-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d5c88-133">响应</span><span class="sxs-lookup"><span data-stu-id="d5c88-133">Response</span></span>
><span data-ttu-id="d5c88-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d5c88-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Accept recommendations accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
