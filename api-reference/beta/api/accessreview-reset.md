---
title: 重置 accessReview
description: 在 "Azure AD 访问评论" 功能中, 重置当前活动的 accessReview 的决策。  目标对象可以是一次性访问评审, 也可以是定期访问评审的实例。  以前的决策不再记录下来, 但审阅者可以继续更新决策。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c8828daf4243ea7bc51a9492944e7fb0a0ed0bd2
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172724"
---
# <a name="reset-accessreview"></a><span data-ttu-id="a7d44-105">重置 accessReview</span><span class="sxs-lookup"><span data-stu-id="a7d44-105">Reset accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7d44-106">在 "Azure AD[访问评论](../resources/accessreviews-root.md)" 功能中, 重置当前活动的[accessReview](../resources/accessreview.md)的决策。</span><span class="sxs-lookup"><span data-stu-id="a7d44-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="a7d44-107">目标对象可以是一次性访问评审, 也可以是定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="a7d44-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="a7d44-108">以前的决策不再记录下来, 但审阅者可以继续更新决策。</span><span class="sxs-lookup"><span data-stu-id="a7d44-108">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7d44-109">权限</span><span class="sxs-lookup"><span data-stu-id="a7d44-109">Permissions</span></span>
<span data-ttu-id="a7d44-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a7d44-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7d44-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7d44-112">Permission type</span></span>                        | <span data-ttu-id="a7d44-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a7d44-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7d44-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7d44-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="a7d44-115">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="a7d44-115">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="a7d44-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7d44-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7d44-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7d44-117">Not supported.</span></span> |
|<span data-ttu-id="a7d44-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7d44-118">Application</span></span>                            | <span data-ttu-id="a7d44-119">AccessReview 的成员资格</span><span class="sxs-lookup"><span data-stu-id="a7d44-119">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7d44-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7d44-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/resetDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="a7d44-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7d44-121">Request headers</span></span>
| <span data-ttu-id="a7d44-122">名称</span><span class="sxs-lookup"><span data-stu-id="a7d44-122">Name</span></span>         | <span data-ttu-id="a7d44-123">类型</span><span class="sxs-lookup"><span data-stu-id="a7d44-123">Type</span></span>        | <span data-ttu-id="a7d44-124">说明</span><span class="sxs-lookup"><span data-stu-id="a7d44-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a7d44-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7d44-125">Authorization</span></span> | <span data-ttu-id="a7d44-126">string</span><span class="sxs-lookup"><span data-stu-id="a7d44-126">string</span></span> | <span data-ttu-id="a7d44-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="a7d44-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7d44-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7d44-129">Request body</span></span>
<span data-ttu-id="a7d44-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a7d44-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a7d44-131">响应</span><span class="sxs-lookup"><span data-stu-id="a7d44-131">Response</span></span>
<span data-ttu-id="a7d44-p105">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a7d44-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7d44-134">示例</span><span class="sxs-lookup"><span data-stu-id="a7d44-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7d44-135">请求</span><span class="sxs-lookup"><span data-stu-id="a7d44-135">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a7d44-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a7d44-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/resetDecisions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a7d44-137">C#</span><span class="sxs-lookup"><span data-stu-id="a7d44-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reset-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a7d44-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="a7d44-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reset-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a7d44-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="a7d44-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reset-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a7d44-140">Java</span><span class="sxs-lookup"><span data-stu-id="a7d44-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reset-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a7d44-141">响应</span><span class="sxs-lookup"><span data-stu-id="a7d44-141">Response</span></span>
><span data-ttu-id="a7d44-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a7d44-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
