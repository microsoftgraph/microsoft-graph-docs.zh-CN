---
title: 获取 accessReviewScheduleDefinition
description: 检索 accessReviewScheduleDefinition 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a6c5619222eb8a96fbf54a8f796abdc2d2bb85ec
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000761"
---
# <a name="get-accessreviewscheduledefinition"></a><span data-ttu-id="6095c-103">获取 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="6095c-103">Get accessReviewScheduleDefinition</span></span>

<span data-ttu-id="6095c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6095c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6095c-105">按 ID 检索 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6095c-105">Retrieve an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object by ID.</span></span> <span data-ttu-id="6095c-106">这将返回除关联的 accessReviewInstances 之外的计划访问审阅系列的所有属性。</span><span class="sxs-lookup"><span data-stu-id="6095c-106">This returns all properties of the scheduled access review series except for the associated accessReviewInstances.</span></span> <span data-ttu-id="6095c-107">每个 accessReviewScheduleDefinition 至少有一个实例。</span><span class="sxs-lookup"><span data-stu-id="6095c-107">Each accessReviewScheduleDefinition has at least one instance.</span></span> <span data-ttu-id="6095c-108">实例表示对特定资源 (（如特定组的成员) ）在一次发生 (（例如，2021年3月) 定期检查）中的审阅。</span><span class="sxs-lookup"><span data-stu-id="6095c-108">An instance represents a review for a specific resource (such as a particular group's members), during one occurrence (e.g., March 2021) of a recurring review.</span></span>

<span data-ttu-id="6095c-109">若要检索访问评审系列的实例，请使用 [List accessReviewInstance](accessreviewinstance-list.md) API。</span><span class="sxs-lookup"><span data-stu-id="6095c-109">To retrieve the instances of the access review series, use the [list accessReviewInstance](accessreviewinstance-list.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="6095c-110">权限</span><span class="sxs-lookup"><span data-stu-id="6095c-110">Permissions</span></span>
<span data-ttu-id="6095c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6095c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6095c-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="6095c-113">Permission type</span></span>                        | <span data-ttu-id="6095c-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6095c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6095c-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6095c-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="6095c-116">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="6095c-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="6095c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6095c-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6095c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6095c-118">Not supported.</span></span>|
|<span data-ttu-id="6095c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="6095c-119">Application</span></span>                            | <span data-ttu-id="6095c-120">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="6095c-120">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="6095c-121">若要调用此 API，登录用户还必须位于允许他们读取访问审核的目录角色中，或者可以将用户作为访问评审的审阅者进行分配。</span><span class="sxs-lookup"><span data-stu-id="6095c-121">To call this API, the signed-in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="6095c-122">有关更多详细信息，请参阅 [access 评审](../resources/accessreviewsv2-root.md)的角色和权限要求。</span><span class="sxs-lookup"><span data-stu-id="6095c-122">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="6095c-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6095c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="6095c-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="6095c-124">Request headers</span></span>
<span data-ttu-id="6095c-125">无。</span><span class="sxs-lookup"><span data-stu-id="6095c-125">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="6095c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6095c-126">Request body</span></span>
<span data-ttu-id="6095c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6095c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6095c-128">响应</span><span class="sxs-lookup"><span data-stu-id="6095c-128">Response</span></span>
<span data-ttu-id="6095c-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6095c-129">If successful, this method returns a `200 OK` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6095c-130">示例</span><span class="sxs-lookup"><span data-stu-id="6095c-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="6095c-131">请求</span><span class="sxs-lookup"><span data-stu-id="6095c-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReviewScheduleDefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
---

### <a name="response"></a><span data-ttu-id="6095c-132">响应</span><span class="sxs-lookup"><span data-stu-id="6095c-132">Response</span></span>
><span data-ttu-id="6095c-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6095c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "60860cdd-fb4d-4054-91ba-f7544443baa6",
    "displayName": "Test world",
    "createdDateTime": "2020-09-14T20:03:36.7391027Z",
    "lastModifiedDateTime": "2020-09-14T20:04:28Z",
    "status": "InProgress",
    "descriptionForAdmins": "",
    "descriptionForReviewers": "",
    "createdBy": {
        "id": "957f1027-c0ee-460d-4444-b8828e59e0fe",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@microsoft.com"
    },
    "scope": {
        "query": "/groups/b7a059cb-038a-4802-8fc9-b944440cf11f/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups/b7a059cb-038a-4802-8fc9-b9d14444f11f",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "None",
        "instanceDurationInDays": 0,
        "autoApplyDecisionsEnabled": false,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": {
                "type": "weekly",
                "interval": 1,
                "month": 0,
                "dayOfMonth": 0,
                "daysOfWeek": [],
                "firstDayOfWeek": "sunday",
                "index": "first"
            },
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2020-09-15",
                "endDate": "9999-12-31"
            }
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="6095c-135">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6095c-135">See also</span></span>

- [<span data-ttu-id="6095c-136">创建 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="6095c-136">Create accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-create.md)
- [<span data-ttu-id="6095c-137">列出 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="6095c-137">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="6095c-138">列出 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="6095c-138">List accessReviewInstance</span></span>](accessreviewinstance-list.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
