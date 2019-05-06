---
title: 列出我的 accessReview 决策
description: 在 "Azure AD 访问评论" 功能中, 检索 accessReview 对象作为审阅者的呼叫用户的决策。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 51eeafd316433678643978b187888e4044d4fbf8
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33586063"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="bccdc-103">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="bccdc-103">List my accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bccdc-104">在 "Azure AD[访问评论](../resources/accessreviews-root.md)" 功能中, 检索[accessReview](../resources/accessreview.md)对象作为审阅者的呼叫用户的决策。</span><span class="sxs-lookup"><span data-stu-id="bccdc-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="bccdc-105">权限</span><span class="sxs-lookup"><span data-stu-id="bccdc-105">Permissions</span></span>
<span data-ttu-id="bccdc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bccdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bccdc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bccdc-108">Permission type</span></span>                        | <span data-ttu-id="bccdc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bccdc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bccdc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bccdc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bccdc-111">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="bccdc-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>   |
|<span data-ttu-id="bccdc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bccdc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bccdc-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bccdc-113">Not supported.</span></span> |
|<span data-ttu-id="bccdc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bccdc-114">Application</span></span>                            | <span data-ttu-id="bccdc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bccdc-115">Not supported.</span></span> |

<span data-ttu-id="bccdc-116">登录用户还必须允许用户阅读此特定访问评审。</span><span class="sxs-lookup"><span data-stu-id="bccdc-116">The signed in user must also be permitted to read this particular access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="bccdc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bccdc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="bccdc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bccdc-118">Request headers</span></span>
| <span data-ttu-id="bccdc-119">名称</span><span class="sxs-lookup"><span data-stu-id="bccdc-119">Name</span></span>         | <span data-ttu-id="bccdc-120">类型</span><span class="sxs-lookup"><span data-stu-id="bccdc-120">Type</span></span>        | <span data-ttu-id="bccdc-121">说明</span><span class="sxs-lookup"><span data-stu-id="bccdc-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bccdc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bccdc-122">Authorization</span></span> | <span data-ttu-id="bccdc-123">string</span><span class="sxs-lookup"><span data-stu-id="bccdc-123">string</span></span> | <span data-ttu-id="bccdc-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="bccdc-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bccdc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bccdc-126">Request body</span></span>
<span data-ttu-id="bccdc-127">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="bccdc-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="bccdc-128">响应</span><span class="sxs-lookup"><span data-stu-id="bccdc-128">Response</span></span>
<span data-ttu-id="bccdc-129">如果成功, 此方法在响应`200, OK`正文中返回响应代码和[accessReviewDecision](../resources/accessreviewdecision.md)对象的数组, 为其调用用户是分配的审阅者。</span><span class="sxs-lookup"><span data-stu-id="bccdc-129">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="bccdc-130">示例</span><span class="sxs-lookup"><span data-stu-id="bccdc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bccdc-131">请求</span><span class="sxs-lookup"><span data-stu-id="bccdc-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```

##### <a name="response"></a><span data-ttu-id="bccdc-132">响应</span><span class="sxs-lookup"><span data-stu-id="bccdc-132">Response</span></span>
><span data-ttu-id="bccdc-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bccdc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewDecision",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
            "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "accessReviewId": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "reviewResult": "Approve",
            "userPrincipalName": "alice@litware.com",
            "userId": "Alice Smith"
    }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bccdc-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="bccdc-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bccdc-136">语言</span><span class="sxs-lookup"><span data-stu-id="bccdc-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bccdc-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="bccdc-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="bccdc-138">另请参阅</span><span class="sxs-lookup"><span data-stu-id="bccdc-138">See also</span></span>

| <span data-ttu-id="bccdc-139">方法</span><span class="sxs-lookup"><span data-stu-id="bccdc-139">Method</span></span>           | <span data-ttu-id="bccdc-140">返回类型</span><span class="sxs-lookup"><span data-stu-id="bccdc-140">Return Type</span></span>    |<span data-ttu-id="bccdc-141">说明</span><span class="sxs-lookup"><span data-stu-id="bccdc-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bccdc-142">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="bccdc-142">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="bccdc-143">accessReview</span><span class="sxs-lookup"><span data-stu-id="bccdc-143">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="bccdc-144">检索访问评审。</span><span class="sxs-lookup"><span data-stu-id="bccdc-144">Retrieve an access review.</span></span> |
|[<span data-ttu-id="bccdc-145">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="bccdc-145">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="bccdc-146">[accessReviewDecision](../resources/accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="bccdc-146">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="bccdc-147">检索 accessReview 的所有决策。</span><span class="sxs-lookup"><span data-stu-id="bccdc-147">Retrieve all the decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listmydecisions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-listmydecisions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
