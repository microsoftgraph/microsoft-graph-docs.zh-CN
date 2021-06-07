---
title: Reset accessReview
description: 在 Azure AD 访问评审功能中，重置当前处于活动状态的 accessReview 的决策。  目标对象可以是一次性访问评审，也可以作为定期访问评审的实例。  不再记录以前的决策，但审阅者可以继续更新决策。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3005c6b8c3fbed81e89de62ff1e3e756cce6bd4a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751027"
---
# <a name="reset-accessreview"></a><span data-ttu-id="7da67-105">Reset accessReview</span><span class="sxs-lookup"><span data-stu-id="7da67-105">Reset accessReview</span></span>

<span data-ttu-id="7da67-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7da67-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7da67-107">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，重置当前处于活动状态的 [accessReview 的决策](../resources/accessreview.md)。</span><span class="sxs-lookup"><span data-stu-id="7da67-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="7da67-108">目标对象可以是一次性访问评审，也可以作为定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="7da67-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="7da67-109">不再记录以前的决策，但审阅者可以继续更新决策。</span><span class="sxs-lookup"><span data-stu-id="7da67-109">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="7da67-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="7da67-110">Permissions</span></span>
<span data-ttu-id="7da67-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7da67-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7da67-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="7da67-113">Permission type</span></span>                        | <span data-ttu-id="7da67-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7da67-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7da67-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7da67-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="7da67-116">AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7da67-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="7da67-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7da67-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7da67-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7da67-118">Not supported.</span></span> |
|<span data-ttu-id="7da67-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="7da67-119">Application</span></span>                            | <span data-ttu-id="7da67-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="7da67-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="7da67-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7da67-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/resetDecisions
```
## <a name="request-headers"></a><span data-ttu-id="7da67-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7da67-122">Request headers</span></span>
| <span data-ttu-id="7da67-123">名称</span><span class="sxs-lookup"><span data-stu-id="7da67-123">Name</span></span>         | <span data-ttu-id="7da67-124">类型</span><span class="sxs-lookup"><span data-stu-id="7da67-124">Type</span></span>        | <span data-ttu-id="7da67-125">说明</span><span class="sxs-lookup"><span data-stu-id="7da67-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7da67-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7da67-126">Authorization</span></span> | <span data-ttu-id="7da67-127">string</span><span class="sxs-lookup"><span data-stu-id="7da67-127">string</span></span> | <span data-ttu-id="7da67-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="7da67-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7da67-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="7da67-130">Request body</span></span>
<span data-ttu-id="7da67-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7da67-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="7da67-132">响应</span><span class="sxs-lookup"><span data-stu-id="7da67-132">Response</span></span>
<span data-ttu-id="7da67-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7da67-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7da67-135">示例</span><span class="sxs-lookup"><span data-stu-id="7da67-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7da67-136">请求</span><span class="sxs-lookup"><span data-stu-id="7da67-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7da67-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7da67-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/resetDecisions
```
# <a name="c"></a>[<span data-ttu-id="7da67-138">C#</span><span class="sxs-lookup"><span data-stu-id="7da67-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reset-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7da67-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7da67-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reset-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7da67-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7da67-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reset-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7da67-141">Java</span><span class="sxs-lookup"><span data-stu-id="7da67-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reset-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7da67-142">响应</span><span class="sxs-lookup"><span data-stu-id="7da67-142">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Reset accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


