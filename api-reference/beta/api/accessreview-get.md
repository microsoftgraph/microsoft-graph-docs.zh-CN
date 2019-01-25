---
title: 获取 accessReview
description: '在 Azure AD 中访问审阅功能，检索 accessReview 对象。  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 26551f27fdf328865509cd02011f3ee2344f5e82
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529143"
---
# <a name="get-accessreview"></a><span data-ttu-id="806e0-103">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="806e0-103">Get accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="806e0-104">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，检索[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="806e0-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="806e0-105">若要检索访问审阅的审阅者，请使用[列表 accessReview 审阅者](accessreview-listreviewers.md)API。</span><span class="sxs-lookup"><span data-stu-id="806e0-105">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="806e0-106">若要检索访问审阅的决策，请使用[列表 accessReview 决策](accessreview-listdecisions.md)API 或[列出我 accessReview 决议](accessreview-listmydecisions.md)API。</span><span class="sxs-lookup"><span data-stu-id="806e0-106">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="806e0-107">如果这是定期访问回顾，然后使用`instances`关系，以检索过去，当前和将来实例访问审阅[accessReview](../resources/accessreview.md)集合。</span><span class="sxs-lookup"><span data-stu-id="806e0-107">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="806e0-108">权限</span><span class="sxs-lookup"><span data-stu-id="806e0-108">Permissions</span></span>
<span data-ttu-id="806e0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="806e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="806e0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="806e0-111">Permission type</span></span>                        | <span data-ttu-id="806e0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="806e0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="806e0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="806e0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="806e0-114">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="806e0-114"></span></span>  <span data-ttu-id="806e0-115">登录的用户也必须在允许他们阅读访问审阅，或作为上访问审阅审阅者分配的目录角色。</span><span class="sxs-lookup"><span data-stu-id="806e0-115">The signed in user must also be in a directory role that permits them to read an access review, or assigned as a reviewer on the access review.</span></span> |
|<span data-ttu-id="806e0-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="806e0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="806e0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="806e0-117">Not supported.</span></span> |
|<span data-ttu-id="806e0-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="806e0-118">Application</span></span>                            | <span data-ttu-id="806e0-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="806e0-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="806e0-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="806e0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="806e0-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="806e0-121">Request headers</span></span>
| <span data-ttu-id="806e0-122">名称</span><span class="sxs-lookup"><span data-stu-id="806e0-122">Name</span></span>         | <span data-ttu-id="806e0-123">类型</span><span class="sxs-lookup"><span data-stu-id="806e0-123">Type</span></span>        | <span data-ttu-id="806e0-124">说明</span><span class="sxs-lookup"><span data-stu-id="806e0-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="806e0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="806e0-125">Authorization</span></span> | <span data-ttu-id="806e0-126">string</span><span class="sxs-lookup"><span data-stu-id="806e0-126">string</span></span> | <span data-ttu-id="806e0-127">持有者令牌</span><span class="sxs-lookup"><span data-stu-id="806e0-127">Bearer \{token\}.</span></span> <span data-ttu-id="806e0-128">必需。</span><span class="sxs-lookup"><span data-stu-id="806e0-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="806e0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="806e0-129">Request body</span></span>
<span data-ttu-id="806e0-130">应提供没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="806e0-130">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="806e0-131">响应</span><span class="sxs-lookup"><span data-stu-id="806e0-131">Response</span></span>
<span data-ttu-id="806e0-132">如果成功，此方法返回`200, OK`响应代码和响应正文中的[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="806e0-132">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="806e0-133">示例</span><span class="sxs-lookup"><span data-stu-id="806e0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="806e0-134">请求</span><span class="sxs-lookup"><span data-stu-id="806e0-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')
```

##### <a name="response"></a><span data-ttu-id="806e0-135">响应</span><span class="sxs-lookup"><span data-stu-id="806e0-135">Response</span></span>
><span data-ttu-id="806e0-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="806e0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"},
    "settings": {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval": true,
        "autoReviewEnabled": false,
        "activityDurationInDays": 30,
        "autoApplyReviewResultsEnabled": false,
        "accessRecommendationsEnabled": false,
        "recurrenceSettings": {
            "recurrenceType": "onetime",
            "recurrenceEndType": "endBy",
            "durationInDays": 0,
            "recurrenceCount": 0
        },
        "autoReviewSettings": {
            "notReviewedResult": "Deny"
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="806e0-138">另请参阅</span><span class="sxs-lookup"><span data-stu-id="806e0-138">See also</span></span>

| <span data-ttu-id="806e0-139">方法</span><span class="sxs-lookup"><span data-stu-id="806e0-139">Method</span></span>           | <span data-ttu-id="806e0-140">返回类型</span><span class="sxs-lookup"><span data-stu-id="806e0-140">Return Type</span></span>    |<span data-ttu-id="806e0-141">说明</span><span class="sxs-lookup"><span data-stu-id="806e0-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="806e0-142">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="806e0-142">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="806e0-143">accessReview</span><span class="sxs-lookup"><span data-stu-id="806e0-143">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="806e0-144">创建新 accessReview。</span><span class="sxs-lookup"><span data-stu-id="806e0-144">Create a new accessReview.</span></span> |
|[<span data-ttu-id="806e0-145">列表 programControls</span><span class="sxs-lookup"><span data-stu-id="806e0-145">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="806e0-146">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="806e0-146">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="806e0-147">列出 programControls 租户中。</span><span class="sxs-lookup"><span data-stu-id="806e0-147">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="806e0-148">列表 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="806e0-148">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="806e0-149">[userIdentity](../resources/useridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="806e0-149">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="806e0-150">要获取 accessReview 审阅的者。</span><span class="sxs-lookup"><span data-stu-id="806e0-150">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="806e0-151">列表 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="806e0-151">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="806e0-152">[accessReviewDecision](../resources/accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="806e0-152">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="806e0-153">获取 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="806e0-153">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="806e0-154">列出我 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="806e0-154">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="806e0-155">[accessReviewDecision](../resources/accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="806e0-155">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="806e0-156">审阅者，以获取 accessReview 我决策。</span><span class="sxs-lookup"><span data-stu-id="806e0-156">As a reviewer, get my decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
