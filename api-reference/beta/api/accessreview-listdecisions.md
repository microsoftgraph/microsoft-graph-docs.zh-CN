---
title: 列表 accessReview 决策
description: 在 Azure AD 中访问审阅功能，检索 accessReview 对象的决策。
localization_priority: Normal
ms.openlocfilehash: ade39abbf63c4e1eb71a6fa25fd3febd8a24c41b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849747"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="da664-103">列表 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="da664-103">List accessReview decisions</span></span>

> <span data-ttu-id="da664-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="da664-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da664-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="da664-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da664-106">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，检索[accessReview](../resources/accessreview.md)对象的决策。</span><span class="sxs-lookup"><span data-stu-id="da664-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="da664-107">请注意，不会进行定期访问回顾`decisions`关系。</span><span class="sxs-lookup"><span data-stu-id="da664-107">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="da664-108">相反，呼叫者必须导航`instance`关系，以查找`accessReview`访问审阅的当前或过去实例的对象。</span><span class="sxs-lookup"><span data-stu-id="da664-108">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="da664-109">权限</span><span class="sxs-lookup"><span data-stu-id="da664-109">Permissions</span></span>
<span data-ttu-id="da664-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da664-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da664-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="da664-112">Permission type</span></span>                        | <span data-ttu-id="da664-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="da664-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="da664-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da664-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="da664-115">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="da664-115"></span></span>  <span data-ttu-id="da664-116">登录的用户还必须在目录角色中允许他们阅读访问审阅。</span><span class="sxs-lookup"><span data-stu-id="da664-116">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="da664-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da664-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da664-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="da664-118">Not supported.</span></span> |
|<span data-ttu-id="da664-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="da664-119">Application</span></span>                            | <span data-ttu-id="da664-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="da664-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da664-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da664-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="da664-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="da664-122">Request headers</span></span>
| <span data-ttu-id="da664-123">名称</span><span class="sxs-lookup"><span data-stu-id="da664-123">Name</span></span>         | <span data-ttu-id="da664-124">类型</span><span class="sxs-lookup"><span data-stu-id="da664-124">Type</span></span>        | <span data-ttu-id="da664-125">说明</span><span class="sxs-lookup"><span data-stu-id="da664-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="da664-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="da664-126">Authorization</span></span> | <span data-ttu-id="da664-127">string</span><span class="sxs-lookup"><span data-stu-id="da664-127">string</span></span> | <span data-ttu-id="da664-128">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="da664-128">Bearer \{token\}.</span></span> <span data-ttu-id="da664-129">必填。</span><span class="sxs-lookup"><span data-stu-id="da664-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da664-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="da664-130">Request body</span></span>
<span data-ttu-id="da664-131">应提供没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="da664-131">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="da664-132">响应</span><span class="sxs-lookup"><span data-stu-id="da664-132">Response</span></span>
<span data-ttu-id="da664-133">如果成功，此方法返回`200, OK`响应代码和响应正文中的[accessReviewDecision](../resources/accessreviewdecision.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="da664-133">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da664-134">示例</span><span class="sxs-lookup"><span data-stu-id="da664-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da664-135">请求</span><span class="sxs-lookup"><span data-stu-id="da664-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/decisions
```

##### <a name="response"></a><span data-ttu-id="da664-136">响应</span><span class="sxs-lookup"><span data-stu-id="da664-136">Response</span></span>
><span data-ttu-id="da664-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="da664-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="da664-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="da664-139">See also</span></span>

| <span data-ttu-id="da664-140">方法</span><span class="sxs-lookup"><span data-stu-id="da664-140">Method</span></span>           | <span data-ttu-id="da664-141">返回类型</span><span class="sxs-lookup"><span data-stu-id="da664-141">Return Type</span></span>    |<span data-ttu-id="da664-142">说明</span><span class="sxs-lookup"><span data-stu-id="da664-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="da664-143">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="da664-143">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="da664-144">accessReview</span><span class="sxs-lookup"><span data-stu-id="da664-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="da664-145">检索访问审阅。</span><span class="sxs-lookup"><span data-stu-id="da664-145">Retrieve an access review.</span></span> |
|[<span data-ttu-id="da664-146">列出我 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="da664-146">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="da664-147">[accessReviewDecision](../resources/accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="da664-147">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="da664-148">审阅者，以获取 accessReview 我决策。</span><span class="sxs-lookup"><span data-stu-id="da664-148">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="da664-149">发送 accessReview 提醒</span><span class="sxs-lookup"><span data-stu-id="da664-149">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="da664-150">无。</span><span class="sxs-lookup"><span data-stu-id="da664-150">None.</span></span>   |   <span data-ttu-id="da664-151">向审阅者的 accessReview 发送提醒。</span><span class="sxs-lookup"><span data-stu-id="da664-151">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="da664-152">停止 accessReview</span><span class="sxs-lookup"><span data-stu-id="da664-152">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="da664-153">无。</span><span class="sxs-lookup"><span data-stu-id="da664-153">None.</span></span>   |   <span data-ttu-id="da664-154">停止 accessReview。</span><span class="sxs-lookup"><span data-stu-id="da664-154">Stop an accessReview.</span></span> |
|[<span data-ttu-id="da664-155">重置 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="da664-155">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="da664-156">无。</span><span class="sxs-lookup"><span data-stu-id="da664-156">None.</span></span>   |   <span data-ttu-id="da664-157">重置正在进行 accessReview 决策。</span><span class="sxs-lookup"><span data-stu-id="da664-157">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="da664-158">应用 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="da664-158">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="da664-159">无。</span><span class="sxs-lookup"><span data-stu-id="da664-159">None.</span></span>   |   <span data-ttu-id="da664-160">应用已完成 accessReview 从的决策。</span><span class="sxs-lookup"><span data-stu-id="da664-160">Apply the decisions from a completed accessReview.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
