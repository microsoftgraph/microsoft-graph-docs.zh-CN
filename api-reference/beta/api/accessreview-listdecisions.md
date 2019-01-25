---
title: 列表 accessReview 决策
description: 在 Azure AD 中访问审阅功能，检索 accessReview 对象的决策。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: eeaa1374bbd44cfe9556e488d25e0fc2c7594cde
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521794"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="60086-103">列表 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="60086-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60086-104">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，检索[accessReview](../resources/accessreview.md)对象的决策。</span><span class="sxs-lookup"><span data-stu-id="60086-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="60086-105">请注意，不会进行定期访问回顾`decisions`关系。</span><span class="sxs-lookup"><span data-stu-id="60086-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="60086-106">相反，呼叫者必须导航`instance`关系，以查找`accessReview`访问审阅的当前或过去实例的对象。</span><span class="sxs-lookup"><span data-stu-id="60086-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="60086-107">权限</span><span class="sxs-lookup"><span data-stu-id="60086-107">Permissions</span></span>
<span data-ttu-id="60086-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60086-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60086-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="60086-110">Permission type</span></span>                        | <span data-ttu-id="60086-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="60086-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="60086-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60086-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="60086-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="60086-113"></span></span>  <span data-ttu-id="60086-114">登录的用户还必须在目录角色中允许他们阅读访问审阅。</span><span class="sxs-lookup"><span data-stu-id="60086-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="60086-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60086-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60086-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="60086-116">Not supported.</span></span> |
|<span data-ttu-id="60086-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="60086-117">Application</span></span>                            | <span data-ttu-id="60086-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="60086-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60086-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60086-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="60086-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="60086-120">Request headers</span></span>
| <span data-ttu-id="60086-121">名称</span><span class="sxs-lookup"><span data-stu-id="60086-121">Name</span></span>         | <span data-ttu-id="60086-122">类型</span><span class="sxs-lookup"><span data-stu-id="60086-122">Type</span></span>        | <span data-ttu-id="60086-123">说明</span><span class="sxs-lookup"><span data-stu-id="60086-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="60086-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="60086-124">Authorization</span></span> | <span data-ttu-id="60086-125">string</span><span class="sxs-lookup"><span data-stu-id="60086-125">string</span></span> | <span data-ttu-id="60086-126">持有者令牌</span><span class="sxs-lookup"><span data-stu-id="60086-126">Bearer \{token\}.</span></span> <span data-ttu-id="60086-127">必需。</span><span class="sxs-lookup"><span data-stu-id="60086-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60086-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="60086-128">Request body</span></span>
<span data-ttu-id="60086-129">应提供没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="60086-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="60086-130">响应</span><span class="sxs-lookup"><span data-stu-id="60086-130">Response</span></span>
<span data-ttu-id="60086-131">如果成功，此方法返回`200, OK`响应代码和响应正文中的[accessReviewDecision](../resources/accessreviewdecision.md)对象的数组。</span><span class="sxs-lookup"><span data-stu-id="60086-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60086-132">示例</span><span class="sxs-lookup"><span data-stu-id="60086-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60086-133">请求</span><span class="sxs-lookup"><span data-stu-id="60086-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/decisions
```

##### <a name="response"></a><span data-ttu-id="60086-134">响应</span><span class="sxs-lookup"><span data-stu-id="60086-134">Response</span></span>
><span data-ttu-id="60086-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="60086-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="60086-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="60086-137">See also</span></span>

| <span data-ttu-id="60086-138">方法</span><span class="sxs-lookup"><span data-stu-id="60086-138">Method</span></span>           | <span data-ttu-id="60086-139">返回类型</span><span class="sxs-lookup"><span data-stu-id="60086-139">Return Type</span></span>    |<span data-ttu-id="60086-140">说明</span><span class="sxs-lookup"><span data-stu-id="60086-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="60086-141">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="60086-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="60086-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="60086-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="60086-143">检索访问审阅。</span><span class="sxs-lookup"><span data-stu-id="60086-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="60086-144">列出我 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="60086-144">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="60086-145">[accessReviewDecision](../resources/accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="60086-145">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="60086-146">审阅者，以获取 accessReview 我决策。</span><span class="sxs-lookup"><span data-stu-id="60086-146">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="60086-147">发送 accessReview 提醒</span><span class="sxs-lookup"><span data-stu-id="60086-147">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="60086-148">无。</span><span class="sxs-lookup"><span data-stu-id="60086-148">None.</span></span>   |   <span data-ttu-id="60086-149">向审阅者的 accessReview 发送提醒。</span><span class="sxs-lookup"><span data-stu-id="60086-149">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="60086-150">停止 accessReview</span><span class="sxs-lookup"><span data-stu-id="60086-150">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="60086-151">无。</span><span class="sxs-lookup"><span data-stu-id="60086-151">None.</span></span>   |   <span data-ttu-id="60086-152">停止 accessReview。</span><span class="sxs-lookup"><span data-stu-id="60086-152">Stop an accessReview.</span></span> |
|[<span data-ttu-id="60086-153">重置 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="60086-153">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="60086-154">无。</span><span class="sxs-lookup"><span data-stu-id="60086-154">None.</span></span>   |   <span data-ttu-id="60086-155">重置正在进行 accessReview 决策。</span><span class="sxs-lookup"><span data-stu-id="60086-155">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="60086-156">应用 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="60086-156">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="60086-157">无。</span><span class="sxs-lookup"><span data-stu-id="60086-157">None.</span></span>   |   <span data-ttu-id="60086-158">应用已完成 accessReview 从的决策。</span><span class="sxs-lookup"><span data-stu-id="60086-158">Apply the decisions from a completed accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listdecisions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
