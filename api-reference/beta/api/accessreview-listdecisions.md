---
title: 列表 accessReview 决策
description: 在 Azure AD 中访问审阅功能，检索 accessReview 对象的决策。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4f89fdbce1c87ce9ef8a6ba8c5b7f9b7be410617
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927007"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="e965c-103">列表 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="e965c-103">List accessReview decisions</span></span>

> <span data-ttu-id="e965c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e965c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e965c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e965c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e965c-106">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，检索[accessReview](../resources/accessreview.md)对象的决策。</span><span class="sxs-lookup"><span data-stu-id="e965c-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="e965c-107">请注意，不会进行定期访问回顾`decisions`关系。</span><span class="sxs-lookup"><span data-stu-id="e965c-107">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="e965c-108">相反，呼叫者必须导航`instance`关系，以查找`accessReview`访问审阅的当前或过去实例的对象。</span><span class="sxs-lookup"><span data-stu-id="e965c-108">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="e965c-109">权限</span><span class="sxs-lookup"><span data-stu-id="e965c-109">Permissions</span></span>
<span data-ttu-id="e965c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e965c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e965c-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e965c-112">Permission type</span></span>                        | <span data-ttu-id="e965c-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e965c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e965c-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e965c-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="e965c-115">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="e965c-115"></span></span>  <span data-ttu-id="e965c-116">登录的用户还必须在目录角色中允许他们阅读访问审阅。</span><span class="sxs-lookup"><span data-stu-id="e965c-116">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="e965c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e965c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e965c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e965c-118">Not supported.</span></span> |
|<span data-ttu-id="e965c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="e965c-119">Application</span></span>                            | <span data-ttu-id="e965c-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="e965c-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e965c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e965c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="e965c-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e965c-122">Request headers</span></span>
| <span data-ttu-id="e965c-123">名称</span><span class="sxs-lookup"><span data-stu-id="e965c-123">Name</span></span>         | <span data-ttu-id="e965c-124">类型</span><span class="sxs-lookup"><span data-stu-id="e965c-124">Type</span></span>        | <span data-ttu-id="e965c-125">说明</span><span class="sxs-lookup"><span data-stu-id="e965c-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e965c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e965c-126">Authorization</span></span> | <span data-ttu-id="e965c-127">string</span><span class="sxs-lookup"><span data-stu-id="e965c-127">string</span></span> | <span data-ttu-id="e965c-128">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="e965c-128">Bearer \{token\}.</span></span> <span data-ttu-id="e965c-129">必需。</span><span class="sxs-lookup"><span data-stu-id="e965c-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e965c-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e965c-130">Request body</span></span>
<span data-ttu-id="e965c-131">应提供没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="e965c-131">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="e965c-132">响应</span><span class="sxs-lookup"><span data-stu-id="e965c-132">Response</span></span>
<span data-ttu-id="e965c-133">如果成功，此方法返回`200, OK`响应代码和响应正文中的[accessReviewDecision](../resources/accessreviewdecision.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="e965c-133">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e965c-134">示例</span><span class="sxs-lookup"><span data-stu-id="e965c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e965c-135">请求</span><span class="sxs-lookup"><span data-stu-id="e965c-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/decisions
```

##### <a name="response"></a><span data-ttu-id="e965c-136">响应</span><span class="sxs-lookup"><span data-stu-id="e965c-136">Response</span></span>
><span data-ttu-id="e965c-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e965c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="e965c-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e965c-139">See also</span></span>

| <span data-ttu-id="e965c-140">方法</span><span class="sxs-lookup"><span data-stu-id="e965c-140">Method</span></span>           | <span data-ttu-id="e965c-141">返回类型</span><span class="sxs-lookup"><span data-stu-id="e965c-141">Return Type</span></span>    |<span data-ttu-id="e965c-142">说明</span><span class="sxs-lookup"><span data-stu-id="e965c-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e965c-143">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="e965c-143">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="e965c-144">accessReview</span><span class="sxs-lookup"><span data-stu-id="e965c-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="e965c-145">检索访问审阅。</span><span class="sxs-lookup"><span data-stu-id="e965c-145">Retrieve an access review.</span></span> |
|[<span data-ttu-id="e965c-146">列出我 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="e965c-146">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="e965c-147">[accessReviewDecision](../resources/accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="e965c-147">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="e965c-148">审阅者，以获取 accessReview 我决策。</span><span class="sxs-lookup"><span data-stu-id="e965c-148">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="e965c-149">发送 accessReview 提醒</span><span class="sxs-lookup"><span data-stu-id="e965c-149">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="e965c-150">无。</span><span class="sxs-lookup"><span data-stu-id="e965c-150">None.</span></span>   |   <span data-ttu-id="e965c-151">向审阅者的 accessReview 发送提醒。</span><span class="sxs-lookup"><span data-stu-id="e965c-151">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="e965c-152">停止 accessReview</span><span class="sxs-lookup"><span data-stu-id="e965c-152">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="e965c-153">无。</span><span class="sxs-lookup"><span data-stu-id="e965c-153">None.</span></span>   |   <span data-ttu-id="e965c-154">停止 accessReview。</span><span class="sxs-lookup"><span data-stu-id="e965c-154">Stop an accessReview.</span></span> |
|[<span data-ttu-id="e965c-155">重置 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="e965c-155">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="e965c-156">无。</span><span class="sxs-lookup"><span data-stu-id="e965c-156">None.</span></span>   |   <span data-ttu-id="e965c-157">重置正在进行 accessReview 决策。</span><span class="sxs-lookup"><span data-stu-id="e965c-157">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="e965c-158">应用 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="e965c-158">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="e965c-159">无。</span><span class="sxs-lookup"><span data-stu-id="e965c-159">None.</span></span>   |   <span data-ttu-id="e965c-160">应用已完成 accessReview 从的决策。</span><span class="sxs-lookup"><span data-stu-id="e965c-160">Apply the decisions from a completed accessReview.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
