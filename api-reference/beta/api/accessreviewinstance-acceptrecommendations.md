---
title: 'accessReviewInstance: acceptRecommendations'
description: '允许接受对他们作为审阅者的访问审核实例上所有未审阅的决策的建议。 '
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a9dee9f65d4070860c2826b64b602984d7d324a1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222165"
---
# <a name="accessreviewinstance-acceptrecommendations"></a><span data-ttu-id="f5d2a-103">accessReviewInstance: acceptRecommendations</span><span class="sxs-lookup"><span data-stu-id="f5d2a-103">accessReviewInstance: acceptRecommendations</span></span>

<span data-ttu-id="f5d2a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5d2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5d2a-105">允许接受对其审阅者的[accessReviewInstance](../resources/accessreviewinstance.md)上所有未审阅的[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)的建议。</span><span class="sxs-lookup"><span data-stu-id="f5d2a-105">Allows the acceptance of recommendations on all not reviewed [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) on an [accessReviewInstance](../resources/accessreviewinstance.md) that they are the reviewer on.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5d2a-106">权限</span><span class="sxs-lookup"><span data-stu-id="f5d2a-106">Permissions</span></span>
<span data-ttu-id="f5d2a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5d2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5d2a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5d2a-109">Permission type</span></span>                        | <span data-ttu-id="f5d2a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f5d2a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5d2a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5d2a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5d2a-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5d2a-112">AccessReview.ReadWrite.All</span></span> |
| <span data-ttu-id="f5d2a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5d2a-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f5d2a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5d2a-114">Not supported.</span></span> |

<span data-ttu-id="f5d2a-115">登录用户还必须是 accessReviewInstance 上的审阅者。</span><span class="sxs-lookup"><span data-stu-id="f5d2a-115">The signed-in user must also be a reviewer on the accessReviewInstance.</span></span>

## <a name="http-request"></a><span data-ttu-id="f5d2a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5d2a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/pendingAccessReviewInstances/{instance-id}/acceptRecommendations
```
## <a name="request-headers"></a><span data-ttu-id="f5d2a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5d2a-117">Request headers</span></span>
<span data-ttu-id="f5d2a-118">无。</span><span class="sxs-lookup"><span data-stu-id="f5d2a-118">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="f5d2a-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5d2a-119">Request body</span></span>
<span data-ttu-id="f5d2a-120">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f5d2a-120">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5d2a-121">响应</span><span class="sxs-lookup"><span data-stu-id="f5d2a-121">Response</span></span>
<span data-ttu-id="f5d2a-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f5d2a-p102">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f5d2a-124">示例</span><span class="sxs-lookup"><span data-stu-id="f5d2a-124">Examples</span></span>
### <a name="request"></a><span data-ttu-id="f5d2a-125">请求</span><span class="sxs-lookup"><span data-stu-id="f5d2a-125">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f5d2a-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5d2a-126">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "acceptrecommendations_accessReviewInstance"
}-->
```http
POST https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/acceptRecommendations
```
# <a name="c"></a>[<span data-ttu-id="f5d2a-127">C#</span><span class="sxs-lookup"><span data-stu-id="f5d2a-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/acceptrecommendations-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5d2a-128">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5d2a-128">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/acceptrecommendations-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5d2a-129">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5d2a-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/acceptrecommendations-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5d2a-130">Java</span><span class="sxs-lookup"><span data-stu-id="f5d2a-130">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/acceptrecommendations-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f5d2a-131">响应</span><span class="sxs-lookup"><span data-stu-id="f5d2a-131">Response</span></span>
><span data-ttu-id="f5d2a-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f5d2a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
