---
title: 列出 accessReviewScheduleDefinitions
description: 检索 accessReviewScheduleDefinition 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3d073dbf0b6f2bdb17fb9649596c6ee04332d81c
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000758"
---
# <a name="list-accessreviewscheduledefinition"></a><span data-ttu-id="4a2cc-103">列出 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="4a2cc-103">List accessReviewScheduleDefinition</span></span>

<span data-ttu-id="4a2cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a2cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a2cc-105">检索 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4a2cc-105">Retrieve the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects.</span></span> <span data-ttu-id="4a2cc-106">将返回零个或多个 accessReviewScheduleDefinition 对象的列表，包括所有已创建的访问评审系列的所有嵌套属性。</span><span class="sxs-lookup"><span data-stu-id="4a2cc-106">A list of zero or more accessReviewScheduleDefinition objects are returned, including all of their nested properties, for each access review series created.</span></span> <span data-ttu-id="4a2cc-107">这不包括关联的 accessReviewInstances。</span><span class="sxs-lookup"><span data-stu-id="4a2cc-107">This does not include associated accessReviewInstances.</span></span>

>[!NOTE]
><span data-ttu-id="4a2cc-108">如果返回多个 **accessReviewScheduleDefinitions** ，则要提高效率并避免超时，请在页面中检索结果集，方法是在页面大小最多为100的情况下包括 $top 查询参数以及请求中的 $skip = 0 查询参数。</span><span class="sxs-lookup"><span data-stu-id="4a2cc-108">If many **accessReviewScheduleDefinitions** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="4a2cc-109">当结果集跨越多个页面时，Microsoft Graph 将在包含指向结果下一页的 URL 的响应中的 nextLink 属性返回该页面，其中包含一个 @odata。</span><span class="sxs-lookup"><span data-stu-id="4a2cc-109">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="4a2cc-110">如果该属性存在，则继续在每个响应中 @odata 使用 nextLink URL 进行额外请求，直到返回所有结果，如您的应用程序中分页 Microsoft Graph 数据中所述。</span><span class="sxs-lookup"><span data-stu-id="4a2cc-110">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="4a2cc-111">如果未提供查询参数，且结果多于100，则 Microsoft Graph 将自动对结果进行分页，每页100个结果。</span><span class="sxs-lookup"><span data-stu-id="4a2cc-111">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>


## <a name="permissions"></a><span data-ttu-id="4a2cc-112">权限</span><span class="sxs-lookup"><span data-stu-id="4a2cc-112">Permissions</span></span>
<span data-ttu-id="4a2cc-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a2cc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a2cc-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a2cc-115">Permission type</span></span>                        | <span data-ttu-id="4a2cc-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4a2cc-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a2cc-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a2cc-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a2cc-118">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="4a2cc-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="4a2cc-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a2cc-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a2cc-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a2cc-120">Not supported.</span></span>|
|<span data-ttu-id="4a2cc-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a2cc-121">Application</span></span>                            | <span data-ttu-id="4a2cc-122">AccessReview、AccessReview 和所有</span><span class="sxs-lookup"><span data-stu-id="4a2cc-122">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

 <span data-ttu-id="4a2cc-123">登录用户还必须位于允许他们阅读访问审核的目录角色中。</span><span class="sxs-lookup"><span data-stu-id="4a2cc-123">The signed-in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="4a2cc-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a2cc-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions
```
## <a name="request-headers"></a><span data-ttu-id="4a2cc-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a2cc-125">Request headers</span></span>
<span data-ttu-id="4a2cc-126">无。</span><span class="sxs-lookup"><span data-stu-id="4a2cc-126">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="4a2cc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a2cc-127">Request body</span></span>
<span data-ttu-id="4a2cc-128">请勿提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="4a2cc-128">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="4a2cc-129">响应</span><span class="sxs-lookup"><span data-stu-id="4a2cc-129">Response</span></span>
<span data-ttu-id="4a2cc-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的数组。</span><span class="sxs-lookup"><span data-stu-id="4a2cc-130">If successful, this method returns a `200 OK` response code and an array of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4a2cc-131">示例</span><span class="sxs-lookup"><span data-stu-id="4a2cc-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="4a2cc-132">请求</span><span class="sxs-lookup"><span data-stu-id="4a2cc-132">Request</span></span>
<span data-ttu-id="4a2cc-133">下面的示例演示检索租户中的所有访问评审系列的请求。</span><span class="sxs-lookup"><span data-stu-id="4a2cc-133">The following example shows a request to retrieve all the access review series in a tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions?$top=100&$skip=0
```
---

### <a name="response"></a><span data-ttu-id="4a2cc-134">响应</span><span class="sxs-lookup"><span data-stu-id="4a2cc-134">Response</span></span>
><span data-ttu-id="4a2cc-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4a2cc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.count": 1,
    "value": [
        {
            "id": "98dcebed-c7f6-46f4-bcf3-4a3fccdb3e2a",
            "displayName": "Access Review",
            "createdDateTime": "2020-09-09T14:27:59Z",
            "lastModifiedDateTime": "2020-09-11T12:02:50Z",
            "status": "InProgress",
            "descriptionForAdmins": "",
            "descriptionForReviewers": "",
            "createdBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "displayName": "MOD Administrator",
                "userPrincipalName": "admin@microsoft.com"
            },
            "scope": {
                "query": "/groups/119cc181-22f0-4e18-8537-264e7524ee0b/transitiveMembers",
                "queryType": "MicrosoftGraph"
            },
            "instanceEnumerationScope": {
                "query": "/groups/119cc181-22f0-4e18-8537-264e7524ee0b",
                "queryType": "MicrosoftGraph"
            },
            "reviewers": [
                {
                    "query": "./manager",
                    "queryType": "MicrosoftGraph",
                    "queryRoot": "decisions"
                }
            ],
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
                        "startDate": "2020-09-11",
                        "endDate": "9999-12-31"
                    }
                }
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="4a2cc-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4a2cc-137">See also</span></span>

- [<span data-ttu-id="4a2cc-138">获取 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="4a2cc-138">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
