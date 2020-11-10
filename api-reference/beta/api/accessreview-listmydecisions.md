---
title: 列出我的 accessReview 决策
description: 在 "Azure AD 访问评论" 功能中，检索 accessReview 对象作为审阅者的呼叫用户的决策。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e92a34429cdde9e9911f309439394d44dfb6fd1e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951875"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="d5b33-103">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="d5b33-103">List my accessReview decisions</span></span>

<span data-ttu-id="d5b33-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5b33-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5b33-105">在 "Azure AD [访问评论](../resources/accessreviews-root.md) " 功能中，检索 [accessReview](../resources/accessreview.md) 对象作为审阅者的呼叫用户的决策。</span><span class="sxs-lookup"><span data-stu-id="d5b33-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="d5b33-106">权限</span><span class="sxs-lookup"><span data-stu-id="d5b33-106">Permissions</span></span>
<span data-ttu-id="d5b33-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5b33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5b33-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5b33-109">Permission type</span></span>                        | <span data-ttu-id="d5b33-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5b33-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5b33-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5b33-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5b33-112">AccessReview、AccessReview、成员身份、AccessReview。所有</span><span class="sxs-lookup"><span data-stu-id="d5b33-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>   |
|<span data-ttu-id="d5b33-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5b33-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5b33-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5b33-114">Not supported.</span></span> |
|<span data-ttu-id="d5b33-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5b33-115">Application</span></span>                            | <span data-ttu-id="d5b33-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5b33-116">Not supported.</span></span> |

<span data-ttu-id="d5b33-117">登录用户还必须允许用户阅读此特定访问评审。</span><span class="sxs-lookup"><span data-stu-id="d5b33-117">The signed in user must also be permitted to read this particular access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="d5b33-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5b33-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="d5b33-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5b33-119">Request headers</span></span>
| <span data-ttu-id="d5b33-120">名称</span><span class="sxs-lookup"><span data-stu-id="d5b33-120">Name</span></span>         | <span data-ttu-id="d5b33-121">类型</span><span class="sxs-lookup"><span data-stu-id="d5b33-121">Type</span></span>        | <span data-ttu-id="d5b33-122">说明</span><span class="sxs-lookup"><span data-stu-id="d5b33-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d5b33-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5b33-123">Authorization</span></span> | <span data-ttu-id="d5b33-124">string</span><span class="sxs-lookup"><span data-stu-id="d5b33-124">string</span></span> | <span data-ttu-id="d5b33-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5b33-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5b33-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5b33-127">Request body</span></span>
<span data-ttu-id="d5b33-128">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5b33-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="d5b33-129">响应</span><span class="sxs-lookup"><span data-stu-id="d5b33-129">Response</span></span>
<span data-ttu-id="d5b33-130">如果成功，此方法在 `200, OK` 响应正文中返回响应代码和 [accessReviewDecision](../resources/accessreviewdecision.md) 对象的数组，为其调用用户是分配的审阅者。</span><span class="sxs-lookup"><span data-stu-id="d5b33-130">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="d5b33-131">示例</span><span class="sxs-lookup"><span data-stu-id="d5b33-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5b33-132">请求</span><span class="sxs-lookup"><span data-stu-id="d5b33-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d5b33-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5b33-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```
# <a name="c"></a>[<span data-ttu-id="d5b33-134">C#</span><span class="sxs-lookup"><span data-stu-id="d5b33-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5b33-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5b33-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5b33-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5b33-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d5b33-137">Java</span><span class="sxs-lookup"><span data-stu-id="d5b33-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-decisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d5b33-138">响应</span><span class="sxs-lookup"><span data-stu-id="d5b33-138">Response</span></span>
><span data-ttu-id="d5b33-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d5b33-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d5b33-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d5b33-141">See also</span></span>

| <span data-ttu-id="d5b33-142">方法</span><span class="sxs-lookup"><span data-stu-id="d5b33-142">Method</span></span>           | <span data-ttu-id="d5b33-143">返回类型</span><span class="sxs-lookup"><span data-stu-id="d5b33-143">Return Type</span></span>    |<span data-ttu-id="d5b33-144">说明</span><span class="sxs-lookup"><span data-stu-id="d5b33-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d5b33-145">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="d5b33-145">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="d5b33-146">accessReview</span><span class="sxs-lookup"><span data-stu-id="d5b33-146">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="d5b33-147">检索访问评审。</span><span class="sxs-lookup"><span data-stu-id="d5b33-147">Retrieve an access review.</span></span> |
|[<span data-ttu-id="d5b33-148">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="d5b33-148">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="d5b33-149">[accessReviewDecision](../resources/accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d5b33-149">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="d5b33-150">检索 accessReview 的所有决策。</span><span class="sxs-lookup"><span data-stu-id="d5b33-150">Retrieve all the decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


