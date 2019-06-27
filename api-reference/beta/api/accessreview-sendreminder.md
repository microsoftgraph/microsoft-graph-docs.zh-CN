---
title: SendReminder accessReview
description: '在 "Azure AD access 评论" 功能中, 向当前活动的 accessReview 的审阅者发送提醒。  目标对象可以是一次性访问评审, 也可以是定期访问评审的实例。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 565ae1a8916686069ad8950d7be4a346fef751d8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258812"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="62937-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="62937-104">SendReminder accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62937-105">在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 向当前活动的[accessReview](../resources/accessreview.md)的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="62937-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="62937-106">目标对象可以是一次性访问评审, 也可以是定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="62937-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="62937-107">权限</span><span class="sxs-lookup"><span data-stu-id="62937-107">Permissions</span></span>
<span data-ttu-id="62937-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62937-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62937-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="62937-110">Permission type</span></span>                        | <span data-ttu-id="62937-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62937-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="62937-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62937-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="62937-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62937-113">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="62937-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62937-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62937-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="62937-115">Not supported.</span></span> |
|<span data-ttu-id="62937-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="62937-116">Application</span></span>                            | <span data-ttu-id="62937-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="62937-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="62937-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62937-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="62937-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="62937-119">Request headers</span></span>
| <span data-ttu-id="62937-120">名称</span><span class="sxs-lookup"><span data-stu-id="62937-120">Name</span></span>         | <span data-ttu-id="62937-121">类型</span><span class="sxs-lookup"><span data-stu-id="62937-121">Type</span></span>        | <span data-ttu-id="62937-122">说明</span><span class="sxs-lookup"><span data-stu-id="62937-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="62937-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="62937-123">Authorization</span></span> | <span data-ttu-id="62937-124">string</span><span class="sxs-lookup"><span data-stu-id="62937-124">string</span></span> | <span data-ttu-id="62937-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="62937-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62937-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="62937-127">Request body</span></span>
<span data-ttu-id="62937-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="62937-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="62937-129">响应</span><span class="sxs-lookup"><span data-stu-id="62937-129">Response</span></span>
<span data-ttu-id="62937-p105">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="62937-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62937-132">示例</span><span class="sxs-lookup"><span data-stu-id="62937-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62937-133">请求</span><span class="sxs-lookup"><span data-stu-id="62937-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/sendReminder
```
##### <a name="response"></a><span data-ttu-id="62937-134">响应</span><span class="sxs-lookup"><span data-stu-id="62937-134">Response</span></span>
><span data-ttu-id="62937-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="62937-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="62937-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="62937-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="62937-138">C#</span><span class="sxs-lookup"><span data-stu-id="62937-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/sendReminder_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62937-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="62937-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/sendReminder_accessReview-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="62937-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="62937-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/sendReminder_accessReview-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "SendReminder accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-sendreminder.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/accessreview-sendreminder.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-sendreminder.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
