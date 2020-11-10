---
title: 列出 accessReview 决策
description: 在 "Azure AD 访问评论" 功能中，检索 accessReview 对象的决策。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6510c16f9d3ec7d03ef15610081b13ad9bc904ce
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951567"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="fbb4c-103">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="fbb4c-103">List accessReview decisions</span></span>

<span data-ttu-id="fbb4c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbb4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbb4c-105">在 "Azure AD [访问评论](../resources/accessreviews-root.md) " 功能中，检索 [accessReview](../resources/accessreview.md) 对象的决策。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="fbb4c-106">请注意，定期访问审核不会有 `decisions` 关系。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-106">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="fbb4c-107">相反，调用方必须导航 `instance` 关系以查找 `accessReview` 访问评审的当前实例或过去实例的对象。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-107">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="fbb4c-108">权限</span><span class="sxs-lookup"><span data-stu-id="fbb4c-108">Permissions</span></span>
<span data-ttu-id="fbb4c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbb4c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fbb4c-111">Permission type</span></span>                        | <span data-ttu-id="fbb4c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fbb4c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbb4c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fbb4c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="fbb4c-114">AccessReview、AccessReview、成员身份、AccessReview。所有</span><span class="sxs-lookup"><span data-stu-id="fbb4c-114">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="fbb4c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fbb4c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbb4c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-116">Not supported.</span></span> |
|<span data-ttu-id="fbb4c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fbb4c-117">Application</span></span>                            | <span data-ttu-id="fbb4c-118">AccessReview、AccessReview、成员身份</span><span class="sxs-lookup"><span data-stu-id="fbb4c-118">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="fbb4c-119">登录用户还必须位于允许他们阅读访问审核的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-119">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="fbb4c-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fbb4c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/decisions
```
## <a name="request-headers"></a><span data-ttu-id="fbb4c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="fbb4c-121">Request headers</span></span>
| <span data-ttu-id="fbb4c-122">名称</span><span class="sxs-lookup"><span data-stu-id="fbb4c-122">Name</span></span>         | <span data-ttu-id="fbb4c-123">类型</span><span class="sxs-lookup"><span data-stu-id="fbb4c-123">Type</span></span>        | <span data-ttu-id="fbb4c-124">说明</span><span class="sxs-lookup"><span data-stu-id="fbb4c-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="fbb4c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbb4c-125">Authorization</span></span> | <span data-ttu-id="fbb4c-126">string</span><span class="sxs-lookup"><span data-stu-id="fbb4c-126">string</span></span> | <span data-ttu-id="fbb4c-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fbb4c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="fbb4c-129">Request body</span></span>
<span data-ttu-id="fbb4c-130">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-130">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="fbb4c-131">响应</span><span class="sxs-lookup"><span data-stu-id="fbb4c-131">Response</span></span>
<span data-ttu-id="fbb4c-132">如果成功，此方法 `200, OK` 在响应正文中返回响应代码和 [accessReviewDecision](../resources/accessreviewdecision.md) 对象的数组。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-132">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbb4c-133">示例</span><span class="sxs-lookup"><span data-stu-id="fbb4c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fbb4c-134">请求</span><span class="sxs-lookup"><span data-stu-id="fbb4c-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fbb4c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fbb4c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```
# <a name="c"></a>[<span data-ttu-id="fbb4c-136">C#</span><span class="sxs-lookup"><span data-stu-id="fbb4c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fbb4c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fbb4c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fbb4c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fbb4c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fbb4c-139">Java</span><span class="sxs-lookup"><span data-stu-id="fbb4c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-decisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fbb4c-140">响应</span><span class="sxs-lookup"><span data-stu-id="fbb4c-140">Response</span></span>
><span data-ttu-id="fbb4c-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="fbb4c-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fbb4c-143">See also</span></span>

| <span data-ttu-id="fbb4c-144">方法</span><span class="sxs-lookup"><span data-stu-id="fbb4c-144">Method</span></span>           | <span data-ttu-id="fbb4c-145">返回类型</span><span class="sxs-lookup"><span data-stu-id="fbb4c-145">Return Type</span></span>    |<span data-ttu-id="fbb4c-146">说明</span><span class="sxs-lookup"><span data-stu-id="fbb4c-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fbb4c-147">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="fbb4c-147">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="fbb4c-148">accessReview</span><span class="sxs-lookup"><span data-stu-id="fbb4c-148">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="fbb4c-149">检索访问评审。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-149">Retrieve an access review.</span></span> |
|[<span data-ttu-id="fbb4c-150">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="fbb4c-150">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="fbb4c-151">[accessReviewDecision](../resources/accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fbb4c-151">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="fbb4c-152">作为审阅者，请 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-152">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="fbb4c-153">发送 accessReview 提醒</span><span class="sxs-lookup"><span data-stu-id="fbb4c-153">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="fbb4c-154">无。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-154">None.</span></span>   |   <span data-ttu-id="fbb4c-155">向 accessReview 的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-155">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="fbb4c-156">停止 accessReview</span><span class="sxs-lookup"><span data-stu-id="fbb4c-156">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="fbb4c-157">无。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-157">None.</span></span>   |   <span data-ttu-id="fbb4c-158">停止 accessReview。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-158">Stop an accessReview.</span></span> |
|[<span data-ttu-id="fbb4c-159">重置 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="fbb4c-159">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="fbb4c-160">无。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-160">None.</span></span>   |   <span data-ttu-id="fbb4c-161">在进行中的 accessReview 中重置决策。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-161">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="fbb4c-162">应用 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="fbb4c-162">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="fbb4c-163">无。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-163">None.</span></span>   |   <span data-ttu-id="fbb4c-164">从已完成的 accessReview 应用决策。</span><span class="sxs-lookup"><span data-stu-id="fbb4c-164">Apply the decisions from a completed accessReview.</span></span>|


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


