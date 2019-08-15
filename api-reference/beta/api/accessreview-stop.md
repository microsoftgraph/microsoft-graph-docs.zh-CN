---
title: 停止 accessReview
description: 在 "Azure AD access 评论" 功能中, 停止当前处于活动状态的 accessReview。  目标对象可以是一次性访问评审, 也可以是定期访问评审的实例。  (若要防止定期访问审核启动以后的实例, 请更新它以更改计划的结束日期)。  在访问审核停止后, 审阅者无法再提供输入, 并且可以应用访问审核决定。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6c1616e811f079726614757732d11cd09ec5ed49
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408774"
---
# <a name="stop-accessreview"></a><span data-ttu-id="f5774-106">停止 accessReview</span><span class="sxs-lookup"><span data-stu-id="f5774-106">Stop accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5774-107">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 停止当前处于活动状态的[accessReview](../resources/accessreview.md)。</span><span class="sxs-lookup"><span data-stu-id="f5774-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="f5774-108">目标对象可以是一次性访问评审, 也可以是定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="f5774-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="f5774-109">(若要防止定期访问审核启动以后的实例, 请[更新它](accessreview-update.md)以更改计划的结束日期)。</span><span class="sxs-lookup"><span data-stu-id="f5774-109">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="f5774-110">在访问审核停止后, 审阅者无法再提供输入, 并且可以应用访问审核决定。</span><span class="sxs-lookup"><span data-stu-id="f5774-110">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="f5774-111">权限</span><span class="sxs-lookup"><span data-stu-id="f5774-111">Permissions</span></span>
<span data-ttu-id="f5774-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5774-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5774-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5774-114">Permission type</span></span>                        | <span data-ttu-id="f5774-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f5774-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5774-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5774-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5774-117">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="f5774-117">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="f5774-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5774-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5774-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5774-119">Not supported.</span></span> |
|<span data-ttu-id="f5774-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5774-120">Application</span></span>                            | <span data-ttu-id="f5774-121">AccessReview 的成员资格</span><span class="sxs-lookup"><span data-stu-id="f5774-121">AccessReview.ReadWrite.Membership</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f5774-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5774-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/stop
```
## <a name="request-headers"></a><span data-ttu-id="f5774-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5774-123">Request headers</span></span>
| <span data-ttu-id="f5774-124">名称</span><span class="sxs-lookup"><span data-stu-id="f5774-124">Name</span></span>         | <span data-ttu-id="f5774-125">类型</span><span class="sxs-lookup"><span data-stu-id="f5774-125">Type</span></span>        | <span data-ttu-id="f5774-126">说明</span><span class="sxs-lookup"><span data-stu-id="f5774-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f5774-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5774-127">Authorization</span></span> | <span data-ttu-id="f5774-128">string</span><span class="sxs-lookup"><span data-stu-id="f5774-128">string</span></span> | <span data-ttu-id="f5774-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="f5774-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5774-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5774-131">Request body</span></span>
<span data-ttu-id="f5774-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f5774-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f5774-133">响应</span><span class="sxs-lookup"><span data-stu-id="f5774-133">Response</span></span>
<span data-ttu-id="f5774-p105">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f5774-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5774-136">示例</span><span class="sxs-lookup"><span data-stu-id="f5774-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5774-137">请求</span><span class="sxs-lookup"><span data-stu-id="f5774-137">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f5774-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f5774-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/stop
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f5774-139">C#</span><span class="sxs-lookup"><span data-stu-id="f5774-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f5774-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5774-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f5774-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="f5774-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f5774-142">响应</span><span class="sxs-lookup"><span data-stu-id="f5774-142">Response</span></span>
><span data-ttu-id="f5774-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f5774-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
