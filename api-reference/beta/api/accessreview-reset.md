---
title: 重置 accessReview
description: 在 "Azure AD 访问评论" 功能中，重置当前活动的 accessReview 的决策。  目标对象可以是一次性访问评审，也可以是定期访问评审的实例。  以前的决策不再记录下来，但审阅者可以继续更新决策。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 05d76043970fad8a6cc3018cabedc734fe6ae92c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952717"
---
# <a name="reset-accessreview"></a><span data-ttu-id="7c2b5-105">重置 accessReview</span><span class="sxs-lookup"><span data-stu-id="7c2b5-105">Reset accessReview</span></span>

<span data-ttu-id="7c2b5-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c2b5-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c2b5-107">在 "Azure AD [访问评论](../resources/accessreviews-root.md) " 功能中，重置当前活动的 [accessReview](../resources/accessreview.md)的决策。</span><span class="sxs-lookup"><span data-stu-id="7c2b5-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="7c2b5-108">目标对象可以是一次性访问评审，也可以是定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="7c2b5-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="7c2b5-109">以前的决策不再记录下来，但审阅者可以继续更新决策。</span><span class="sxs-lookup"><span data-stu-id="7c2b5-109">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c2b5-110">权限</span><span class="sxs-lookup"><span data-stu-id="7c2b5-110">Permissions</span></span>
<span data-ttu-id="7c2b5-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c2b5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c2b5-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c2b5-113">Permission type</span></span>                        | <span data-ttu-id="7c2b5-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c2b5-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c2b5-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c2b5-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c2b5-116">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="7c2b5-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="7c2b5-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c2b5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c2b5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c2b5-118">Not supported.</span></span> |
|<span data-ttu-id="7c2b5-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c2b5-119">Application</span></span>                            | <span data-ttu-id="7c2b5-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="7c2b5-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c2b5-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c2b5-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/resetDecisions
```
## <a name="request-headers"></a><span data-ttu-id="7c2b5-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c2b5-122">Request headers</span></span>
| <span data-ttu-id="7c2b5-123">名称</span><span class="sxs-lookup"><span data-stu-id="7c2b5-123">Name</span></span>         | <span data-ttu-id="7c2b5-124">类型</span><span class="sxs-lookup"><span data-stu-id="7c2b5-124">Type</span></span>        | <span data-ttu-id="7c2b5-125">说明</span><span class="sxs-lookup"><span data-stu-id="7c2b5-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7c2b5-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c2b5-126">Authorization</span></span> | <span data-ttu-id="7c2b5-127">string</span><span class="sxs-lookup"><span data-stu-id="7c2b5-127">string</span></span> | <span data-ttu-id="7c2b5-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c2b5-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c2b5-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c2b5-130">Request body</span></span>
<span data-ttu-id="7c2b5-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7c2b5-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="7c2b5-132">响应</span><span class="sxs-lookup"><span data-stu-id="7c2b5-132">Response</span></span>
<span data-ttu-id="7c2b5-p105">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7c2b5-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c2b5-135">示例</span><span class="sxs-lookup"><span data-stu-id="7c2b5-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c2b5-136">请求</span><span class="sxs-lookup"><span data-stu-id="7c2b5-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7c2b5-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c2b5-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/resetDecisions
```
# <a name="c"></a>[<span data-ttu-id="7c2b5-138">C#</span><span class="sxs-lookup"><span data-stu-id="7c2b5-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reset-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c2b5-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c2b5-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reset-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c2b5-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c2b5-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reset-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c2b5-141">Java</span><span class="sxs-lookup"><span data-stu-id="7c2b5-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reset-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7c2b5-142">响应</span><span class="sxs-lookup"><span data-stu-id="7c2b5-142">Response</span></span>
><span data-ttu-id="7c2b5-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7c2b5-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


