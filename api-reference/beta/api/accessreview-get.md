---
title: 获取 accessReview
description: 在 "Azure AD 访问评论" 功能中，检索 accessReview 对象。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bc47fa2d371f2ab0dbcd150aa0005a3cbc82cdac
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951709"
---
# <a name="get-accessreview"></a><span data-ttu-id="85a3d-103">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="85a3d-103">Get accessReview</span></span>

<span data-ttu-id="85a3d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85a3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85a3d-105">在 "Azure AD [访问评论](../resources/accessreviews-root.md) " 功能中，检索 [accessReview](../resources/accessreview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="85a3d-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="85a3d-106">若要检索访问评审的审阅者，请使用 [列表 accessReview 审阅者](accessreview-listreviewers.md) API。</span><span class="sxs-lookup"><span data-stu-id="85a3d-106">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="85a3d-107">若要检索访问评审的决策，请使用 [List accessReview 决策](accessreview-listdecisions.md) api 或 [list my accessReview 决策](accessreview-listmydecisions.md) api。</span><span class="sxs-lookup"><span data-stu-id="85a3d-107">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="85a3d-108">如果这是定期访问审核，则不会将任何决策与定期访问评审系列相关联。</span><span class="sxs-lookup"><span data-stu-id="85a3d-108">If this is a recurring access review, no decisions will be associated with the recurring access review series.</span></span> <span data-ttu-id="85a3d-109">而是使用 `instances` 该系列的关系检索访问评审的过去、当前和未来实例的 [accessReview](../resources/accessreview.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="85a3d-109">Instead, use the `instances` relationship of that series to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span> <span data-ttu-id="85a3d-110">每个过去和当前实例都将做出决策。</span><span class="sxs-lookup"><span data-stu-id="85a3d-110">Each past and current instance will have decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="85a3d-111">权限</span><span class="sxs-lookup"><span data-stu-id="85a3d-111">Permissions</span></span>
<span data-ttu-id="85a3d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85a3d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85a3d-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="85a3d-114">Permission type</span></span>                        | <span data-ttu-id="85a3d-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="85a3d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="85a3d-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85a3d-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="85a3d-117">AccessReview、AccessReview、成员身份、AccessReview。所有</span><span class="sxs-lookup"><span data-stu-id="85a3d-117">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="85a3d-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85a3d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85a3d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="85a3d-119">Not supported.</span></span> |
|<span data-ttu-id="85a3d-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="85a3d-120">Application</span></span>                            | <span data-ttu-id="85a3d-121">AccessReview、AccessReview、成员身份</span><span class="sxs-lookup"><span data-stu-id="85a3d-121">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |

<span data-ttu-id="85a3d-122">若要调用此 API，登录用户还必须位于允许他们读取访问审核的目录角色中，或者可以将用户作为访问评审的审阅者进行分配。</span><span class="sxs-lookup"><span data-stu-id="85a3d-122">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="85a3d-123">有关更多详细信息，请参阅 [access 评审](../resources/accessreviews-root.md)的角色和权限要求。</span><span class="sxs-lookup"><span data-stu-id="85a3d-123">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="85a3d-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85a3d-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="85a3d-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="85a3d-125">Request headers</span></span>
| <span data-ttu-id="85a3d-126">名称</span><span class="sxs-lookup"><span data-stu-id="85a3d-126">Name</span></span>         | <span data-ttu-id="85a3d-127">类型</span><span class="sxs-lookup"><span data-stu-id="85a3d-127">Type</span></span>        | <span data-ttu-id="85a3d-128">说明</span><span class="sxs-lookup"><span data-stu-id="85a3d-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="85a3d-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="85a3d-129">Authorization</span></span> | <span data-ttu-id="85a3d-130">string</span><span class="sxs-lookup"><span data-stu-id="85a3d-130">string</span></span> | <span data-ttu-id="85a3d-p105">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="85a3d-p105">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85a3d-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="85a3d-133">Request body</span></span>
<span data-ttu-id="85a3d-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="85a3d-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85a3d-135">响应</span><span class="sxs-lookup"><span data-stu-id="85a3d-135">Response</span></span>
<span data-ttu-id="85a3d-136">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [accessReview](../resources/accessreview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="85a3d-136">If successful, this method returns a `200 OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85a3d-137">示例</span><span class="sxs-lookup"><span data-stu-id="85a3d-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85a3d-138">请求</span><span class="sxs-lookup"><span data-stu-id="85a3d-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="85a3d-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="85a3d-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
# <a name="c"></a>[<span data-ttu-id="85a3d-140">C#</span><span class="sxs-lookup"><span data-stu-id="85a3d-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85a3d-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85a3d-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85a3d-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85a3d-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85a3d-143">Java</span><span class="sxs-lookup"><span data-stu-id="85a3d-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="85a3d-144">响应</span><span class="sxs-lookup"><span data-stu-id="85a3d-144">Response</span></span>
><span data-ttu-id="85a3d-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="85a3d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="85a3d-147">另请参阅</span><span class="sxs-lookup"><span data-stu-id="85a3d-147">See also</span></span>

- [<span data-ttu-id="85a3d-148">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="85a3d-148">Create accessReview</span></span>](accessreview-create.md)
- [<span data-ttu-id="85a3d-149">列出 accessReviews</span><span class="sxs-lookup"><span data-stu-id="85a3d-149">List accessReviews</span></span>](accessreview-list.md)
- [<span data-ttu-id="85a3d-150">列出 programControls</span><span class="sxs-lookup"><span data-stu-id="85a3d-150">List programControls</span></span>](programcontrol-list.md)
- [<span data-ttu-id="85a3d-151">列出 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="85a3d-151">List accessReview reviewers</span></span>](accessreview-listreviewers.md)
- [<span data-ttu-id="85a3d-152">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="85a3d-152">List accessReview decisions</span></span>](accessreview-listdecisions.md)
- [<span data-ttu-id="85a3d-153">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="85a3d-153">List my accessReview decisions</span></span>](accessreview-listmydecisions.md)


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


