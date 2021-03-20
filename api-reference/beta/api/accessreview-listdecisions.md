---
title: 列出 accessReview 决策
description: 在 Azure AD 访问评审功能中，检索 accessReview 对象的决策。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 74ac3d2d9ec8857333beb94d8c5c96f1c4684c6b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943161"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="72c62-103">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="72c62-103">List accessReview decisions</span></span>

<span data-ttu-id="72c62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72c62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72c62-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，检索 [accessReview 对象](../resources/accessreview.md) 的决策。</span><span class="sxs-lookup"><span data-stu-id="72c62-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="72c62-106">请注意，定期访问评审没有 `decisions` 关系。</span><span class="sxs-lookup"><span data-stu-id="72c62-106">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="72c62-107">相反，调用方必须导航 `instance` 关系以查找访问评审 `accessReview` 的当前或过去实例的对象。</span><span class="sxs-lookup"><span data-stu-id="72c62-107">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="72c62-108">权限</span><span class="sxs-lookup"><span data-stu-id="72c62-108">Permissions</span></span>
<span data-ttu-id="72c62-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72c62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72c62-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="72c62-111">Permission type</span></span>                        | <span data-ttu-id="72c62-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="72c62-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="72c62-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72c62-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="72c62-114">AccessReview.Read.All、AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72c62-114">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="72c62-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72c62-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72c62-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="72c62-116">Not supported.</span></span> |
|<span data-ttu-id="72c62-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="72c62-117">Application</span></span>                            | <span data-ttu-id="72c62-118">AccessReview.Read.All、AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="72c62-118">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="72c62-119">登录用户还必须具有允许其阅读访问评审的目录角色。</span><span class="sxs-lookup"><span data-stu-id="72c62-119">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="72c62-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72c62-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/decisions
```
## <a name="request-headers"></a><span data-ttu-id="72c62-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="72c62-121">Request headers</span></span>
| <span data-ttu-id="72c62-122">名称</span><span class="sxs-lookup"><span data-stu-id="72c62-122">Name</span></span>         | <span data-ttu-id="72c62-123">类型</span><span class="sxs-lookup"><span data-stu-id="72c62-123">Type</span></span>        | <span data-ttu-id="72c62-124">说明</span><span class="sxs-lookup"><span data-stu-id="72c62-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="72c62-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="72c62-125">Authorization</span></span> | <span data-ttu-id="72c62-126">string</span><span class="sxs-lookup"><span data-stu-id="72c62-126">string</span></span> | <span data-ttu-id="72c62-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="72c62-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72c62-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="72c62-129">Request body</span></span>
<span data-ttu-id="72c62-130">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="72c62-130">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="72c62-131">响应</span><span class="sxs-lookup"><span data-stu-id="72c62-131">Response</span></span>
<span data-ttu-id="72c62-132">如果成功，此方法在响应正文中返回 响应代码和 `200, OK` [accessReviewDecision](../resources/accessreviewdecision.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="72c62-132">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72c62-133">示例</span><span class="sxs-lookup"><span data-stu-id="72c62-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72c62-134">请求</span><span class="sxs-lookup"><span data-stu-id="72c62-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="72c62-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="72c62-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```
# <a name="c"></a>[<span data-ttu-id="72c62-136">C#</span><span class="sxs-lookup"><span data-stu-id="72c62-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72c62-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72c62-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72c62-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72c62-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72c62-139">Java</span><span class="sxs-lookup"><span data-stu-id="72c62-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-decisions-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="72c62-140">响应</span><span class="sxs-lookup"><span data-stu-id="72c62-140">Response</span></span>
><span data-ttu-id="72c62-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="72c62-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="72c62-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="72c62-143">See also</span></span>

| <span data-ttu-id="72c62-144">方法</span><span class="sxs-lookup"><span data-stu-id="72c62-144">Method</span></span>           | <span data-ttu-id="72c62-145">返回类型</span><span class="sxs-lookup"><span data-stu-id="72c62-145">Return Type</span></span>    |<span data-ttu-id="72c62-146">说明</span><span class="sxs-lookup"><span data-stu-id="72c62-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="72c62-147">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="72c62-147">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="72c62-148">accessReview</span><span class="sxs-lookup"><span data-stu-id="72c62-148">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="72c62-149">检索访问评审。</span><span class="sxs-lookup"><span data-stu-id="72c62-149">Retrieve an access review.</span></span> |
|[<span data-ttu-id="72c62-150">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="72c62-150">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="72c62-151">[accessReviewDecision](../resources/accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72c62-151">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="72c62-152">作为审阅者，获取我在 accessReview 上的决定。</span><span class="sxs-lookup"><span data-stu-id="72c62-152">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="72c62-153">发送 accessReview 提醒</span><span class="sxs-lookup"><span data-stu-id="72c62-153">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="72c62-154">无。</span><span class="sxs-lookup"><span data-stu-id="72c62-154">None.</span></span>   |   <span data-ttu-id="72c62-155">向 accessReview 的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="72c62-155">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="72c62-156">Stop accessReview</span><span class="sxs-lookup"><span data-stu-id="72c62-156">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="72c62-157">无。</span><span class="sxs-lookup"><span data-stu-id="72c62-157">None.</span></span>   |   <span data-ttu-id="72c62-158">停止 accessReview。</span><span class="sxs-lookup"><span data-stu-id="72c62-158">Stop an accessReview.</span></span> |
|[<span data-ttu-id="72c62-159">重置 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="72c62-159">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="72c62-160">无。</span><span class="sxs-lookup"><span data-stu-id="72c62-160">None.</span></span>   |   <span data-ttu-id="72c62-161">重置进行中的 accessReview 中的决策。</span><span class="sxs-lookup"><span data-stu-id="72c62-161">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="72c62-162">应用 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="72c62-162">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="72c62-163">无。</span><span class="sxs-lookup"><span data-stu-id="72c62-163">None.</span></span>   |   <span data-ttu-id="72c62-164">从已完成的 accessReview 应用决策。</span><span class="sxs-lookup"><span data-stu-id="72c62-164">Apply the decisions from a completed accessReview.</span></span>|


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


