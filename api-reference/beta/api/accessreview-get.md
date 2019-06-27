---
title: 获取 accessReview
description: '在 "Azure AD 访问评论" 功能中, 检索 accessReview 对象。  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 34236a1c8d80aa48976a4fcb65c503b5b7ab7a2c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258966"
---
# <a name="get-accessreview"></a><span data-ttu-id="7353e-103">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="7353e-103">Get accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7353e-104">在 "Azure AD[访问评论](../resources/accessreviews-root.md)" 功能中, 检索[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7353e-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="7353e-105">若要检索访问评审的审阅者, 请使用[列表 accessReview 审阅者](accessreview-listreviewers.md)API。</span><span class="sxs-lookup"><span data-stu-id="7353e-105">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="7353e-106">若要检索访问评审的决策, 请使用[List accessReview 决策](accessreview-listdecisions.md)api 或[list my accessReview 决策](accessreview-listmydecisions.md)api。</span><span class="sxs-lookup"><span data-stu-id="7353e-106">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="7353e-107">如果这是定期访问审核, 则使用`instances`关系检索访问评审的过去、当前和未来实例的[accessReview](../resources/accessreview.md)集合。</span><span class="sxs-lookup"><span data-stu-id="7353e-107">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="7353e-108">权限</span><span class="sxs-lookup"><span data-stu-id="7353e-108">Permissions</span></span>
<span data-ttu-id="7353e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7353e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7353e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7353e-111">Permission type</span></span>                        | <span data-ttu-id="7353e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7353e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7353e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7353e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7353e-114">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="7353e-114">AccessReview.Read.All</span></span>  |
|<span data-ttu-id="7353e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7353e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7353e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7353e-116">Not supported.</span></span> |
|<span data-ttu-id="7353e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7353e-117">Application</span></span>                            | <span data-ttu-id="7353e-118">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="7353e-118">AccessReview.Read.All</span></span>  |

<span data-ttu-id="7353e-119">若要调用此 API, 登录用户还必须位于允许他们读取访问审核的目录角色中, 或者可以将用户作为访问评审的审阅者进行分配。</span><span class="sxs-lookup"><span data-stu-id="7353e-119">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="7353e-120">有关更多详细信息, 请参阅[access 评审](../resources/accessreviews-root.md)的角色和权限要求。</span><span class="sxs-lookup"><span data-stu-id="7353e-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="7353e-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7353e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="7353e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7353e-122">Request headers</span></span>
| <span data-ttu-id="7353e-123">名称</span><span class="sxs-lookup"><span data-stu-id="7353e-123">Name</span></span>         | <span data-ttu-id="7353e-124">类型</span><span class="sxs-lookup"><span data-stu-id="7353e-124">Type</span></span>        | <span data-ttu-id="7353e-125">说明</span><span class="sxs-lookup"><span data-stu-id="7353e-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7353e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7353e-126">Authorization</span></span> | <span data-ttu-id="7353e-127">string</span><span class="sxs-lookup"><span data-stu-id="7353e-127">string</span></span> | <span data-ttu-id="7353e-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="7353e-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7353e-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="7353e-130">Request body</span></span>
<span data-ttu-id="7353e-131">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="7353e-131">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="7353e-132">响应</span><span class="sxs-lookup"><span data-stu-id="7353e-132">Response</span></span>
<span data-ttu-id="7353e-133">如果成功, 此方法在响应`200, OK`正文中返回响应代码和[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7353e-133">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7353e-134">示例</span><span class="sxs-lookup"><span data-stu-id="7353e-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7353e-135">请求</span><span class="sxs-lookup"><span data-stu-id="7353e-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
```

##### <a name="response"></a><span data-ttu-id="7353e-136">响应</span><span class="sxs-lookup"><span data-stu-id="7353e-136">Response</span></span>
><span data-ttu-id="7353e-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7353e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7353e-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7353e-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7353e-140">C#</span><span class="sxs-lookup"><span data-stu-id="7353e-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7353e-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="7353e-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_accessReview-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7353e-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="7353e-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_accessReview-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="7353e-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7353e-143">See also</span></span>

| <span data-ttu-id="7353e-144">方法</span><span class="sxs-lookup"><span data-stu-id="7353e-144">Method</span></span>           | <span data-ttu-id="7353e-145">返回类型</span><span class="sxs-lookup"><span data-stu-id="7353e-145">Return Type</span></span>    |<span data-ttu-id="7353e-146">说明</span><span class="sxs-lookup"><span data-stu-id="7353e-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7353e-147">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="7353e-147">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="7353e-148">accessReview</span><span class="sxs-lookup"><span data-stu-id="7353e-148">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="7353e-149">创建新的 accessReview。</span><span class="sxs-lookup"><span data-stu-id="7353e-149">Create a new accessReview.</span></span> |
|[<span data-ttu-id="7353e-150">列出 programControls</span><span class="sxs-lookup"><span data-stu-id="7353e-150">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="7353e-151">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="7353e-151">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="7353e-152">列出租户中的 programControls。</span><span class="sxs-lookup"><span data-stu-id="7353e-152">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="7353e-153">列出 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="7353e-153">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="7353e-154">[userIdentity](../resources/useridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="7353e-154">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="7353e-155">获取 accessReview 的审阅者。</span><span class="sxs-lookup"><span data-stu-id="7353e-155">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="7353e-156">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="7353e-156">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="7353e-157">[accessReviewDecision](../resources/accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="7353e-157">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="7353e-158">获取 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="7353e-158">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="7353e-159">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="7353e-159">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="7353e-160">[accessReviewDecision](../resources/accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="7353e-160">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="7353e-161">作为审阅者, 请 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="7353e-161">As a reviewer, get my decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/accessreview-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
