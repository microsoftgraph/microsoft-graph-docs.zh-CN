---
title: 列出 accessReview 决策
description: 在 "Azure AD 访问评论" 功能中, 检索 accessReview 对象的决策。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fee4b4adc4bc4e33964575976c67cfeaa077a34c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323722"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="b5f7e-103">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="b5f7e-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5f7e-104">在 "Azure AD[访问评论](../resources/accessreviews-root.md)" 功能中, 检索[accessReview](../resources/accessreview.md)对象的决策。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="b5f7e-105">请注意, 定期访问审核不会有`decisions`关系。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="b5f7e-106">相反, 调用方必须导航`instance`关系以查找访问评审`accessReview`的当前实例或过去实例的对象。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5f7e-107">权限</span><span class="sxs-lookup"><span data-stu-id="b5f7e-107">Permissions</span></span>
<span data-ttu-id="b5f7e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5f7e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5f7e-110">Permission type</span></span>                        | <span data-ttu-id="b5f7e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5f7e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5f7e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5f7e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5f7e-113">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="b5f7e-113">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="b5f7e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5f7e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5f7e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-115">Not supported.</span></span> |
|<span data-ttu-id="b5f7e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5f7e-116">Application</span></span>                            | <span data-ttu-id="b5f7e-117">AccessReview</span><span class="sxs-lookup"><span data-stu-id="b5f7e-117">AccessReview.Read.All</span></span> |

 <span data-ttu-id="b5f7e-118">登录用户还必须位于允许他们阅读访问审核的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-118">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="b5f7e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5f7e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="b5f7e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5f7e-120">Request headers</span></span>
| <span data-ttu-id="b5f7e-121">名称</span><span class="sxs-lookup"><span data-stu-id="b5f7e-121">Name</span></span>         | <span data-ttu-id="b5f7e-122">类型</span><span class="sxs-lookup"><span data-stu-id="b5f7e-122">Type</span></span>        | <span data-ttu-id="b5f7e-123">说明</span><span class="sxs-lookup"><span data-stu-id="b5f7e-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b5f7e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5f7e-124">Authorization</span></span> | <span data-ttu-id="b5f7e-125">string</span><span class="sxs-lookup"><span data-stu-id="b5f7e-125">string</span></span> | <span data-ttu-id="b5f7e-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5f7e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5f7e-128">Request body</span></span>
<span data-ttu-id="b5f7e-129">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="b5f7e-130">响应</span><span class="sxs-lookup"><span data-stu-id="b5f7e-130">Response</span></span>
<span data-ttu-id="b5f7e-131">如果成功, 此方法在响应`200, OK`正文中返回响应代码和[accessReviewDecision](../resources/accessreviewdecision.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5f7e-132">示例</span><span class="sxs-lookup"><span data-stu-id="b5f7e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5f7e-133">请求</span><span class="sxs-lookup"><span data-stu-id="b5f7e-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```

##### <a name="response"></a><span data-ttu-id="b5f7e-134">响应</span><span class="sxs-lookup"><span data-stu-id="b5f7e-134">Response</span></span>
><span data-ttu-id="b5f7e-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="b5f7e-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b5f7e-137">See also</span></span>

| <span data-ttu-id="b5f7e-138">方法</span><span class="sxs-lookup"><span data-stu-id="b5f7e-138">Method</span></span>           | <span data-ttu-id="b5f7e-139">返回类型</span><span class="sxs-lookup"><span data-stu-id="b5f7e-139">Return Type</span></span>    |<span data-ttu-id="b5f7e-140">说明</span><span class="sxs-lookup"><span data-stu-id="b5f7e-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b5f7e-141">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="b5f7e-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="b5f7e-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="b5f7e-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="b5f7e-143">检索访问评审。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="b5f7e-144">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="b5f7e-144">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="b5f7e-145">[accessReviewDecision](../resources/accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="b5f7e-145">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="b5f7e-146">作为审阅者, 请 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-146">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="b5f7e-147">发送 accessReview 提醒</span><span class="sxs-lookup"><span data-stu-id="b5f7e-147">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="b5f7e-148">无。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-148">None.</span></span>   |   <span data-ttu-id="b5f7e-149">向 accessReview 的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-149">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="b5f7e-150">停止 accessReview</span><span class="sxs-lookup"><span data-stu-id="b5f7e-150">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="b5f7e-151">无。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-151">None.</span></span>   |   <span data-ttu-id="b5f7e-152">停止 accessReview。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-152">Stop an accessReview.</span></span> |
|[<span data-ttu-id="b5f7e-153">重置 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="b5f7e-153">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="b5f7e-154">无。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-154">None.</span></span>   |   <span data-ttu-id="b5f7e-155">在进行中的 accessReview 中重置决策。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-155">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="b5f7e-156">应用 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="b5f7e-156">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="b5f7e-157">无。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-157">None.</span></span>   |   <span data-ttu-id="b5f7e-158">从已完成的 accessReview 应用决策。</span><span class="sxs-lookup"><span data-stu-id="b5f7e-158">Apply the decisions from a completed accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
