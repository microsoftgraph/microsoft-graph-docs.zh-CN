---
title: 列出 accessReview 决策
description: 在 "Azure AD 访问评论" 功能中, 检索 accessReview 对象的决策。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b82b3fc19320d1a4a1f4f77c18f5ad866f0a8cab
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172713"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="9e317-103">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="9e317-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e317-104">在 "Azure AD[访问评论](../resources/accessreviews-root.md)" 功能中, 检索[accessReview](../resources/accessreview.md)对象的决策。</span><span class="sxs-lookup"><span data-stu-id="9e317-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="9e317-105">请注意, 定期访问审核不会有`decisions`关系。</span><span class="sxs-lookup"><span data-stu-id="9e317-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="9e317-106">相反, 调用方必须导航`instance`关系以查找访问评审`accessReview`的当前实例或过去实例的对象。</span><span class="sxs-lookup"><span data-stu-id="9e317-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e317-107">权限</span><span class="sxs-lookup"><span data-stu-id="9e317-107">Permissions</span></span>
<span data-ttu-id="9e317-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9e317-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e317-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e317-110">Permission type</span></span>                        | <span data-ttu-id="9e317-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9e317-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e317-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e317-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9e317-113">AccessReview、AccessReview、成员身份、AccessReview。所有</span><span class="sxs-lookup"><span data-stu-id="9e317-113">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="9e317-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e317-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e317-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e317-115">Not supported.</span></span> |
|<span data-ttu-id="9e317-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e317-116">Application</span></span>                            | <span data-ttu-id="9e317-117">AccessReview、AccessReview、成员身份</span><span class="sxs-lookup"><span data-stu-id="9e317-117">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="9e317-118">登录用户还必须位于允许他们阅读访问审核的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="9e317-118">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="9e317-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e317-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="9e317-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e317-120">Request headers</span></span>
| <span data-ttu-id="9e317-121">名称</span><span class="sxs-lookup"><span data-stu-id="9e317-121">Name</span></span>         | <span data-ttu-id="9e317-122">类型</span><span class="sxs-lookup"><span data-stu-id="9e317-122">Type</span></span>        | <span data-ttu-id="9e317-123">说明</span><span class="sxs-lookup"><span data-stu-id="9e317-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9e317-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e317-124">Authorization</span></span> | <span data-ttu-id="9e317-125">string</span><span class="sxs-lookup"><span data-stu-id="9e317-125">string</span></span> | <span data-ttu-id="9e317-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="9e317-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e317-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e317-128">Request body</span></span>
<span data-ttu-id="9e317-129">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="9e317-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="9e317-130">响应</span><span class="sxs-lookup"><span data-stu-id="9e317-130">Response</span></span>
<span data-ttu-id="9e317-131">如果成功, 此方法在响应`200, OK`正文中返回响应代码和[accessReviewDecision](../resources/accessreviewdecision.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="9e317-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e317-132">示例</span><span class="sxs-lookup"><span data-stu-id="9e317-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e317-133">请求</span><span class="sxs-lookup"><span data-stu-id="9e317-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9e317-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="9e317-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9e317-135">C#</span><span class="sxs-lookup"><span data-stu-id="9e317-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9e317-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="9e317-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9e317-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="9e317-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9e317-138">Java</span><span class="sxs-lookup"><span data-stu-id="9e317-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-decisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9e317-139">响应</span><span class="sxs-lookup"><span data-stu-id="9e317-139">Response</span></span>
><span data-ttu-id="9e317-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9e317-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="9e317-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9e317-142">See also</span></span>

| <span data-ttu-id="9e317-143">方法</span><span class="sxs-lookup"><span data-stu-id="9e317-143">Method</span></span>           | <span data-ttu-id="9e317-144">返回类型</span><span class="sxs-lookup"><span data-stu-id="9e317-144">Return Type</span></span>    |<span data-ttu-id="9e317-145">说明</span><span class="sxs-lookup"><span data-stu-id="9e317-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9e317-146">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="9e317-146">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="9e317-147">accessReview</span><span class="sxs-lookup"><span data-stu-id="9e317-147">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="9e317-148">检索访问评审。</span><span class="sxs-lookup"><span data-stu-id="9e317-148">Retrieve an access review.</span></span> |
|[<span data-ttu-id="9e317-149">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="9e317-149">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="9e317-150">[accessReviewDecision](../resources/accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="9e317-150">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="9e317-151">作为审阅者, 请 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="9e317-151">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="9e317-152">发送 accessReview 提醒</span><span class="sxs-lookup"><span data-stu-id="9e317-152">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="9e317-153">无。</span><span class="sxs-lookup"><span data-stu-id="9e317-153">None.</span></span>   |   <span data-ttu-id="9e317-154">向 accessReview 的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="9e317-154">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="9e317-155">停止 accessReview</span><span class="sxs-lookup"><span data-stu-id="9e317-155">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="9e317-156">无。</span><span class="sxs-lookup"><span data-stu-id="9e317-156">None.</span></span>   |   <span data-ttu-id="9e317-157">停止 accessReview。</span><span class="sxs-lookup"><span data-stu-id="9e317-157">Stop an accessReview.</span></span> |
|[<span data-ttu-id="9e317-158">重置 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="9e317-158">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="9e317-159">无。</span><span class="sxs-lookup"><span data-stu-id="9e317-159">None.</span></span>   |   <span data-ttu-id="9e317-160">在进行中的 accessReview 中重置决策。</span><span class="sxs-lookup"><span data-stu-id="9e317-160">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="9e317-161">应用 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="9e317-161">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="9e317-162">无。</span><span class="sxs-lookup"><span data-stu-id="9e317-162">None.</span></span>   |   <span data-ttu-id="9e317-163">从已完成的 accessReview 应用决策。</span><span class="sxs-lookup"><span data-stu-id="9e317-163">Apply the decisions from a completed accessReview.</span></span>|


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
