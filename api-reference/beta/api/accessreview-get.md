---
title: 获取 accessReview
description: '在 Azure AD 中访问审阅功能，检索 accessReview 对象。  '
localization_priority: Normal
ms.openlocfilehash: 471cebe3dbfa60e6cc05e2be546504216163ee0f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894038"
---
# <a name="get-accessreview"></a><span data-ttu-id="d904e-103">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="d904e-103">Get accessReview</span></span>

> <span data-ttu-id="d904e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d904e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d904e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d904e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d904e-106">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，检索[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d904e-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="d904e-107">若要检索访问审阅的审阅者，请使用[列表 accessReview 审阅者](accessreview-listreviewers.md)API。</span><span class="sxs-lookup"><span data-stu-id="d904e-107">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="d904e-108">若要检索访问审阅的决策，请使用[列表 accessReview 决策](accessreview-listdecisions.md)API 或[列出我 accessReview 决议](accessreview-listmydecisions.md)API。</span><span class="sxs-lookup"><span data-stu-id="d904e-108">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="d904e-109">如果这是定期访问回顾，然后使用`instances`关系，以检索过去，当前和将来实例访问审阅[accessReview](../resources/accessreview.md)集合。</span><span class="sxs-lookup"><span data-stu-id="d904e-109">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="d904e-110">权限</span><span class="sxs-lookup"><span data-stu-id="d904e-110">Permissions</span></span>
<span data-ttu-id="d904e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d904e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d904e-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="d904e-113">Permission type</span></span>                        | <span data-ttu-id="d904e-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d904e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d904e-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d904e-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="d904e-116">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="d904e-116"></span></span>  <span data-ttu-id="d904e-117">登录的用户也必须在目录角色，它允许他们阅读访问审阅，或作为上访问审阅审阅者分配。</span><span class="sxs-lookup"><span data-stu-id="d904e-117">The signed in user must also be in a directory role which permits them to read an access review, or assigned as a reviewer on the access review.</span></span> |
|<span data-ttu-id="d904e-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d904e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d904e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d904e-119">Not supported.</span></span> |
|<span data-ttu-id="d904e-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="d904e-120">Application</span></span>                            | <span data-ttu-id="d904e-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="d904e-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d904e-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d904e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="d904e-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d904e-123">Request headers</span></span>
| <span data-ttu-id="d904e-124">名称</span><span class="sxs-lookup"><span data-stu-id="d904e-124">Name</span></span>         | <span data-ttu-id="d904e-125">类型</span><span class="sxs-lookup"><span data-stu-id="d904e-125">Type</span></span>        | <span data-ttu-id="d904e-126">说明</span><span class="sxs-lookup"><span data-stu-id="d904e-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d904e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d904e-127">Authorization</span></span> | <span data-ttu-id="d904e-128">string</span><span class="sxs-lookup"><span data-stu-id="d904e-128">string</span></span> | <span data-ttu-id="d904e-129">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="d904e-129">Bearer \{token\}.</span></span> <span data-ttu-id="d904e-130">必填。</span><span class="sxs-lookup"><span data-stu-id="d904e-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d904e-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="d904e-131">Request body</span></span>
<span data-ttu-id="d904e-132">应提供没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="d904e-132">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="d904e-133">响应</span><span class="sxs-lookup"><span data-stu-id="d904e-133">Response</span></span>
<span data-ttu-id="d904e-134">如果成功，此方法返回`200, OK`响应代码和响应正文中的[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d904e-134">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d904e-135">示例</span><span class="sxs-lookup"><span data-stu-id="d904e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d904e-136">请求</span><span class="sxs-lookup"><span data-stu-id="d904e-136">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')
```

##### <a name="response"></a><span data-ttu-id="d904e-137">响应</span><span class="sxs-lookup"><span data-stu-id="d904e-137">Response</span></span>
><span data-ttu-id="d904e-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d904e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
    "displayName": "review",
    "startDateTime": "2017-11-14T01:14:54.89Z",
    "endDateTime": "2017-12-14T01:14:54.89Z",
    "status": "InProgress",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "self",
    "description": "",
    "settings": {
        "reviewId": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval": true,
        "recurrenceSettings": {
            "recurrenceType": "onetime",
            "recurrenceEndType": "endBy",
            "durationInDays": 0,
            "recurrenceCount": 0
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="d904e-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d904e-140">See also</span></span>

| <span data-ttu-id="d904e-141">方法</span><span class="sxs-lookup"><span data-stu-id="d904e-141">Method</span></span>           | <span data-ttu-id="d904e-142">返回类型</span><span class="sxs-lookup"><span data-stu-id="d904e-142">Return Type</span></span>    |<span data-ttu-id="d904e-143">说明</span><span class="sxs-lookup"><span data-stu-id="d904e-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d904e-144">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="d904e-144">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="d904e-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="d904e-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="d904e-146">创建新 accessReview。</span><span class="sxs-lookup"><span data-stu-id="d904e-146">Create a new accessReview.</span></span> |
|[<span data-ttu-id="d904e-147">列表 programControls</span><span class="sxs-lookup"><span data-stu-id="d904e-147">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="d904e-148">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="d904e-148">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="d904e-149">列出 programControls 租户中。</span><span class="sxs-lookup"><span data-stu-id="d904e-149">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="d904e-150">列表 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="d904e-150">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="d904e-151">[userIdentity](../resources/useridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="d904e-151">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="d904e-152">要获取 accessReview 审阅的者。</span><span class="sxs-lookup"><span data-stu-id="d904e-152">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="d904e-153">列表 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="d904e-153">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="d904e-154">[accessReviewDecision](../resources/accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="d904e-154">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="d904e-155">获取 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="d904e-155">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="d904e-156">列出我 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="d904e-156">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="d904e-157">[accessReviewDecision](../resources/accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="d904e-157">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="d904e-158">审阅者，以获取 accessReview 我决策。</span><span class="sxs-lookup"><span data-stu-id="d904e-158">As a reviewer, get my decisions of an accessReview.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
