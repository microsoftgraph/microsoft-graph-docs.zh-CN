---
title: 获取 accessReview
description: 在 Azure AD 访问评审功能中，检索 accessReview 对象。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 01bf052e6e77377c5ec07eddfc005b1a05394106
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048496"
---
# <a name="get-accessreview"></a><span data-ttu-id="1199b-103">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="1199b-103">Get accessReview</span></span>

<span data-ttu-id="1199b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1199b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1199b-105">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，检索 [accessReview](../resources/accessreview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1199b-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="1199b-106">若要检索访问评审的审阅者，请使用 [列表 accessReview reviewers](accessreview-listreviewers.md) API。</span><span class="sxs-lookup"><span data-stu-id="1199b-106">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="1199b-107">若要检索访问评审的决策，请使用 [列表 accessReview 决策](accessreview-listdecisions.md) API 或列表 [my accessReview 决策](accessreview-listmydecisions.md) API。</span><span class="sxs-lookup"><span data-stu-id="1199b-107">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="1199b-108">如果这是定期访问评审，则不与定期访问评审系列关联任何决策。</span><span class="sxs-lookup"><span data-stu-id="1199b-108">If this is a recurring access review, no decisions will be associated with the recurring access review series.</span></span> <span data-ttu-id="1199b-109">相反，请使用该系列的关系检索访问评审的过去、当前和未来实例的 `instances` [accessReview](../resources/accessreview.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="1199b-109">Instead, use the `instances` relationship of that series to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span> <span data-ttu-id="1199b-110">每个过去和当前实例都将有决策。</span><span class="sxs-lookup"><span data-stu-id="1199b-110">Each past and current instance will have decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="1199b-111">权限</span><span class="sxs-lookup"><span data-stu-id="1199b-111">Permissions</span></span>
<span data-ttu-id="1199b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1199b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1199b-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="1199b-114">Permission type</span></span>                        | <span data-ttu-id="1199b-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1199b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1199b-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1199b-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="1199b-117">AccessReview.Read.All、AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1199b-117">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="1199b-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1199b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1199b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="1199b-119">Not supported.</span></span> |
|<span data-ttu-id="1199b-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="1199b-120">Application</span></span>                            | <span data-ttu-id="1199b-121">AccessReview.Read.All、AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="1199b-121">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |

<span data-ttu-id="1199b-122">为了调用此 API，已登录用户还必须位于允许他们阅读访问评审的目录角色中，或者可以将该用户分配为访问评审的审阅者。</span><span class="sxs-lookup"><span data-stu-id="1199b-122">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="1199b-123">有关详细信息，请参阅访问评审的角色和 [权限要求](../resources/accessreviews-root.md)。</span><span class="sxs-lookup"><span data-stu-id="1199b-123">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="1199b-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1199b-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="1199b-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="1199b-125">Request headers</span></span>
| <span data-ttu-id="1199b-126">名称</span><span class="sxs-lookup"><span data-stu-id="1199b-126">Name</span></span>         | <span data-ttu-id="1199b-127">类型</span><span class="sxs-lookup"><span data-stu-id="1199b-127">Type</span></span>        | <span data-ttu-id="1199b-128">说明</span><span class="sxs-lookup"><span data-stu-id="1199b-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1199b-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="1199b-129">Authorization</span></span> | <span data-ttu-id="1199b-130">string</span><span class="sxs-lookup"><span data-stu-id="1199b-130">string</span></span> | <span data-ttu-id="1199b-p105">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="1199b-p105">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1199b-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="1199b-133">Request body</span></span>
<span data-ttu-id="1199b-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1199b-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1199b-135">响应</span><span class="sxs-lookup"><span data-stu-id="1199b-135">Response</span></span>
<span data-ttu-id="1199b-136">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [accessReview](../resources/accessreview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1199b-136">If successful, this method returns a `200 OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1199b-137">示例</span><span class="sxs-lookup"><span data-stu-id="1199b-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1199b-138">请求</span><span class="sxs-lookup"><span data-stu-id="1199b-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1199b-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="1199b-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
# <a name="c"></a>[<span data-ttu-id="1199b-140">C#</span><span class="sxs-lookup"><span data-stu-id="1199b-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1199b-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1199b-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1199b-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1199b-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1199b-143">Java</span><span class="sxs-lookup"><span data-stu-id="1199b-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1199b-144">响应</span><span class="sxs-lookup"><span data-stu-id="1199b-144">Response</span></span>
><span data-ttu-id="1199b-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1199b-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="1199b-146">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1199b-146">See also</span></span>

- [<span data-ttu-id="1199b-147">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="1199b-147">Create accessReview</span></span>](accessreview-create.md)
- [<span data-ttu-id="1199b-148">列出 accessReviews</span><span class="sxs-lookup"><span data-stu-id="1199b-148">List accessReviews</span></span>](accessreview-list.md)
- [<span data-ttu-id="1199b-149">列出 programControls</span><span class="sxs-lookup"><span data-stu-id="1199b-149">List programControls</span></span>](programcontrol-list.md)
- [<span data-ttu-id="1199b-150">列出 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="1199b-150">List accessReview reviewers</span></span>](accessreview-listreviewers.md)
- [<span data-ttu-id="1199b-151">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="1199b-151">List accessReview decisions</span></span>](accessreview-listdecisions.md)
- [<span data-ttu-id="1199b-152">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="1199b-152">List my accessReview decisions</span></span>](accessreview-listmydecisions.md)


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


