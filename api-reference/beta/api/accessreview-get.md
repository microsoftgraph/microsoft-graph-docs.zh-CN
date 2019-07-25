---
title: 获取 accessReview
description: '在 "Azure AD 访问评论" 功能中, 检索 accessReview 对象。  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 032265b8764aef1c4ce00c765f0215fdd9c8fe9b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856049"
---
# <a name="get-accessreview"></a><span data-ttu-id="f8746-103">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="f8746-103">Get accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8746-104">在 "Azure AD[访问评论](../resources/accessreviews-root.md)" 功能中, 检索[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f8746-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="f8746-105">若要检索访问评审的审阅者, 请使用[列表 accessReview 审阅者](accessreview-listreviewers.md)API。</span><span class="sxs-lookup"><span data-stu-id="f8746-105">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="f8746-106">若要检索访问评审的决策, 请使用[List accessReview 决策](accessreview-listdecisions.md)api 或[list my accessReview 决策](accessreview-listmydecisions.md)api。</span><span class="sxs-lookup"><span data-stu-id="f8746-106">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="f8746-107">如果这是定期访问审核, 则使用`instances`关系检索访问评审的过去、当前和未来实例的[accessReview](../resources/accessreview.md)集合。</span><span class="sxs-lookup"><span data-stu-id="f8746-107">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8746-108">权限</span><span class="sxs-lookup"><span data-stu-id="f8746-108">Permissions</span></span>
<span data-ttu-id="f8746-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8746-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8746-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8746-111">Permission type</span></span>                        | <span data-ttu-id="f8746-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8746-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8746-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8746-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8746-114">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8746-114">AccessReview.Read.All</span></span>  |
|<span data-ttu-id="f8746-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8746-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8746-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8746-116">Not supported.</span></span> |
|<span data-ttu-id="f8746-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8746-117">Application</span></span>                            | <span data-ttu-id="f8746-118">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8746-118">AccessReview.Read.All</span></span>  |

<span data-ttu-id="f8746-119">若要调用此 API, 登录用户还必须位于允许他们读取访问审核的目录角色中, 或者可以将用户作为访问评审的审阅者进行分配。</span><span class="sxs-lookup"><span data-stu-id="f8746-119">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="f8746-120">有关更多详细信息, 请参阅[access 评审](../resources/accessreviews-root.md)的角色和权限要求。</span><span class="sxs-lookup"><span data-stu-id="f8746-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="f8746-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8746-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="f8746-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8746-122">Request headers</span></span>
| <span data-ttu-id="f8746-123">名称</span><span class="sxs-lookup"><span data-stu-id="f8746-123">Name</span></span>         | <span data-ttu-id="f8746-124">类型</span><span class="sxs-lookup"><span data-stu-id="f8746-124">Type</span></span>        | <span data-ttu-id="f8746-125">说明</span><span class="sxs-lookup"><span data-stu-id="f8746-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f8746-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8746-126">Authorization</span></span> | <span data-ttu-id="f8746-127">string</span><span class="sxs-lookup"><span data-stu-id="f8746-127">string</span></span> | <span data-ttu-id="f8746-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8746-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8746-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8746-130">Request body</span></span>
<span data-ttu-id="f8746-131">不应提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="f8746-131">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="f8746-132">响应</span><span class="sxs-lookup"><span data-stu-id="f8746-132">Response</span></span>
<span data-ttu-id="f8746-133">如果成功, 此方法在响应`200, OK`正文中返回响应代码和[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f8746-133">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8746-134">示例</span><span class="sxs-lookup"><span data-stu-id="f8746-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8746-135">请求</span><span class="sxs-lookup"><span data-stu-id="f8746-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f8746-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f8746-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f8746-137">C#</span><span class="sxs-lookup"><span data-stu-id="f8746-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f8746-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="f8746-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f8746-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="f8746-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f8746-140">Java</span><span class="sxs-lookup"><span data-stu-id="f8746-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f8746-141">响应</span><span class="sxs-lookup"><span data-stu-id="f8746-141">Response</span></span>
><span data-ttu-id="f8746-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f8746-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="f8746-144">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f8746-144">See also</span></span>

| <span data-ttu-id="f8746-145">方法</span><span class="sxs-lookup"><span data-stu-id="f8746-145">Method</span></span>           | <span data-ttu-id="f8746-146">返回类型</span><span class="sxs-lookup"><span data-stu-id="f8746-146">Return Type</span></span>    |<span data-ttu-id="f8746-147">说明</span><span class="sxs-lookup"><span data-stu-id="f8746-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f8746-148">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="f8746-148">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="f8746-149">accessReview</span><span class="sxs-lookup"><span data-stu-id="f8746-149">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="f8746-150">创建新的 accessReview。</span><span class="sxs-lookup"><span data-stu-id="f8746-150">Create a new accessReview.</span></span> |
|[<span data-ttu-id="f8746-151">列出 programControls</span><span class="sxs-lookup"><span data-stu-id="f8746-151">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="f8746-152">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="f8746-152">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="f8746-153">列出租户中的 programControls。</span><span class="sxs-lookup"><span data-stu-id="f8746-153">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="f8746-154">列出 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="f8746-154">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="f8746-155">[userIdentity](../resources/useridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="f8746-155">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="f8746-156">获取 accessReview 的审阅者。</span><span class="sxs-lookup"><span data-stu-id="f8746-156">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="f8746-157">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="f8746-157">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="f8746-158">[accessReviewDecision](../resources/accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="f8746-158">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="f8746-159">获取 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="f8746-159">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="f8746-160">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="f8746-160">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="f8746-161">[accessReviewDecision](../resources/accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="f8746-161">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="f8746-162">作为审阅者, 请 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="f8746-162">As a reviewer, get my decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
