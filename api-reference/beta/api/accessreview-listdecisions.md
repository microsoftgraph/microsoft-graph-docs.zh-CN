---
title: 列出 accessReview 决策
description: 在 Azure AD 访问评审功能中，检索 accessReview 对象的决策。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 23813096fb625e9598347bde0628c7dd6f407296
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751109"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="318b9-103">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="318b9-103">List accessReview decisions</span></span>

<span data-ttu-id="318b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="318b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="318b9-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，检索 [accessReview 对象](../resources/accessreview.md) 的决策。</span><span class="sxs-lookup"><span data-stu-id="318b9-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="318b9-106">请注意，定期访问评审 **将没有决策** 关系。</span><span class="sxs-lookup"><span data-stu-id="318b9-106">Note that a recurring access review will not have a **decisions** relationship.</span></span>  <span data-ttu-id="318b9-107">相反，调用方必须导航 **实例** 关系以查找访问评审的当前或过去实例的 [accessReview](../resources/accessreview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="318b9-107">Instead, the caller must navigate the **instance** relationship to find an [accessReview](../resources/accessreview.md) object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="318b9-108">权限</span><span class="sxs-lookup"><span data-stu-id="318b9-108">Permissions</span></span>
<span data-ttu-id="318b9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="318b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="318b9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="318b9-111">Permission type</span></span>                        | <span data-ttu-id="318b9-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="318b9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="318b9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="318b9-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="318b9-114">AccessReview.Read.All、AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="318b9-114">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="318b9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="318b9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="318b9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="318b9-116">Not supported.</span></span> |
|<span data-ttu-id="318b9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="318b9-117">Application</span></span>                            | <span data-ttu-id="318b9-118">AccessReview.Read.All、AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="318b9-118">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="318b9-119">登录用户还必须具有允许其阅读访问评审的目录角色。</span><span class="sxs-lookup"><span data-stu-id="318b9-119">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="318b9-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="318b9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/decisions
```
## <a name="request-headers"></a><span data-ttu-id="318b9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="318b9-121">Request headers</span></span>
| <span data-ttu-id="318b9-122">名称</span><span class="sxs-lookup"><span data-stu-id="318b9-122">Name</span></span>         | <span data-ttu-id="318b9-123">类型</span><span class="sxs-lookup"><span data-stu-id="318b9-123">Type</span></span>        | <span data-ttu-id="318b9-124">说明</span><span class="sxs-lookup"><span data-stu-id="318b9-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="318b9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="318b9-125">Authorization</span></span> | <span data-ttu-id="318b9-126">string</span><span class="sxs-lookup"><span data-stu-id="318b9-126">string</span></span> | <span data-ttu-id="318b9-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="318b9-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="318b9-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="318b9-129">Request body</span></span>
<span data-ttu-id="318b9-130">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="318b9-130">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="318b9-131">响应</span><span class="sxs-lookup"><span data-stu-id="318b9-131">Response</span></span>
<span data-ttu-id="318b9-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewDecision](../resources/accessreviewdecision.md) 对象数组。</span><span class="sxs-lookup"><span data-stu-id="318b9-132">If successful, this method returns a `200 OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="318b9-133">示例</span><span class="sxs-lookup"><span data-stu-id="318b9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="318b9-134">请求</span><span class="sxs-lookup"><span data-stu-id="318b9-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="318b9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="318b9-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```
# <a name="c"></a>[<span data-ttu-id="318b9-136">C#</span><span class="sxs-lookup"><span data-stu-id="318b9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="318b9-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="318b9-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="318b9-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="318b9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="318b9-139">Java</span><span class="sxs-lookup"><span data-stu-id="318b9-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-decisions-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="318b9-140">响应</span><span class="sxs-lookup"><span data-stu-id="318b9-140">Response</span></span>
><span data-ttu-id="318b9-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="318b9-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="318b9-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="318b9-142">See also</span></span>

| <span data-ttu-id="318b9-143">方法</span><span class="sxs-lookup"><span data-stu-id="318b9-143">Method</span></span>           | <span data-ttu-id="318b9-144">返回类型</span><span class="sxs-lookup"><span data-stu-id="318b9-144">Return Type</span></span>    |<span data-ttu-id="318b9-145">说明</span><span class="sxs-lookup"><span data-stu-id="318b9-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="318b9-146">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="318b9-146">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="318b9-147">accessReview</span><span class="sxs-lookup"><span data-stu-id="318b9-147">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="318b9-148">检索访问评审。</span><span class="sxs-lookup"><span data-stu-id="318b9-148">Retrieve an access review.</span></span> |
|[<span data-ttu-id="318b9-149">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="318b9-149">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="318b9-150">[accessReviewDecision](../resources/accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="318b9-150">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="318b9-151">作为审阅者，获取我在 accessReview 上的决定。</span><span class="sxs-lookup"><span data-stu-id="318b9-151">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="318b9-152">发送 accessReview 提醒</span><span class="sxs-lookup"><span data-stu-id="318b9-152">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="318b9-153">无。</span><span class="sxs-lookup"><span data-stu-id="318b9-153">None.</span></span>   |   <span data-ttu-id="318b9-154">向 accessReview 的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="318b9-154">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="318b9-155">Stop accessReview</span><span class="sxs-lookup"><span data-stu-id="318b9-155">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="318b9-156">无。</span><span class="sxs-lookup"><span data-stu-id="318b9-156">None.</span></span>   |   <span data-ttu-id="318b9-157">停止 accessReview。</span><span class="sxs-lookup"><span data-stu-id="318b9-157">Stop an accessReview.</span></span> |
|[<span data-ttu-id="318b9-158">重置 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="318b9-158">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="318b9-159">无。</span><span class="sxs-lookup"><span data-stu-id="318b9-159">None.</span></span>   |   <span data-ttu-id="318b9-160">重置进行中的 accessReview 中的决策。</span><span class="sxs-lookup"><span data-stu-id="318b9-160">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="318b9-161">应用 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="318b9-161">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="318b9-162">无。</span><span class="sxs-lookup"><span data-stu-id="318b9-162">None.</span></span>   |   <span data-ttu-id="318b9-163">从已完成的 accessReview 应用决策。</span><span class="sxs-lookup"><span data-stu-id="318b9-163">Apply the decisions from a completed accessReview.</span></span>|


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


