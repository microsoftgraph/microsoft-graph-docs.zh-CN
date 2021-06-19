---
title: accessReviewScheduleDefinition： filterByCurrentUser
description: 返回 accessReviewScheduleDefinition 对象，其中调用用户是审阅者。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 45ffe40876fc1a569383e788056a73692fe46a34
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031438"
---
# <a name="accessreviewscheduledefinition-filterbycurrentuser"></a><span data-ttu-id="20632-103">accessReviewScheduleDefinition： filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="20632-103">accessReviewScheduleDefinition: filterByCurrentUser</span></span>
<span data-ttu-id="20632-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20632-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20632-105">返回 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象，其中调用用户是一个或多个 [accessReviewInstance](../resources/accessreviewinstance.md) 对象的审阅者。</span><span class="sxs-lookup"><span data-stu-id="20632-105">Returns [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects where the calling user is a reviewer on one or more [accessReviewInstance](../resources/accessreviewinstance.md) objects.</span></span>

>[!NOTE]
><span data-ttu-id="20632-106">此 API 的默认页面大小为 100 accessReviewScheduleDefinition 对象。</span><span class="sxs-lookup"><span data-stu-id="20632-106">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="20632-107">若要提高效率并避免由于大型结果集而超时，请通过使用 和 查询参数应用 `$skip` `$top` 分页。</span><span class="sxs-lookup"><span data-stu-id="20632-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="20632-108">有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="20632-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="20632-109">权限</span><span class="sxs-lookup"><span data-stu-id="20632-109">Permissions</span></span>
<span data-ttu-id="20632-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20632-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20632-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="20632-112">Permission type</span></span>|<span data-ttu-id="20632-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20632-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20632-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20632-114">Delegated (work or school account)</span></span>|<span data-ttu-id="20632-115">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20632-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="20632-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20632-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20632-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="20632-117">Not supported.</span></span>|
|<span data-ttu-id="20632-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="20632-118">Application</span></span>|<span data-ttu-id="20632-119">AccessReview.Read.All、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20632-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20632-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20632-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/filterByCurrentUser(on='reviewer')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20632-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="20632-121">Optional query parameters</span></span>
<span data-ttu-id="20632-122">此方法支持 `$select` 、 、 、 和 OData 查询参数 `$filter` `$orderBy` `$skip` `$top` 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="20632-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="20632-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="20632-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="20632-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="20632-124">Request headers</span></span>
|<span data-ttu-id="20632-125">名称</span><span class="sxs-lookup"><span data-stu-id="20632-125">Name</span></span>|<span data-ttu-id="20632-126">说明</span><span class="sxs-lookup"><span data-stu-id="20632-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="20632-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="20632-127">Authorization</span></span>|<span data-ttu-id="20632-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="20632-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20632-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="20632-130">Request body</span></span>
<span data-ttu-id="20632-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="20632-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20632-132">响应</span><span class="sxs-lookup"><span data-stu-id="20632-132">Response</span></span>

<span data-ttu-id="20632-133">如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="20632-133">If successful, this function returns a `200 OK` response code and a [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20632-134">示例</span><span class="sxs-lookup"><span data-stu-id="20632-134">Examples</span></span>
<span data-ttu-id="20632-135">返回调用用户是审阅者的所有审阅定义。</span><span class="sxs-lookup"><span data-stu-id="20632-135">Returns all review definitions where the calling user is a reviewer.</span></span>

### <a name="request"></a><span data-ttu-id="20632-136">请求</span><span class="sxs-lookup"><span data-stu-id="20632-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewscheduledefinition_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/filterByCurrentUser(on='reviewer')
```


### <a name="response"></a><span data-ttu-id="20632-137">响应</span><span class="sxs-lookup"><span data-stu-id="20632-137">Response</span></span>
><span data-ttu-id="20632-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="20632-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewScheduleDefinition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(accessReviewScheduleDefinition)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewScheduleDefinition",
            "id": "ad0ec492-c1b6-49f0-9025-ea15ca471ea9",
            "displayName": "Test",
            "createdDateTime": "2021-04-29T20:01:18.1084432Z",
            "lastModifiedDateTime": "2021-04-29T20:01:52.3233462Z",
            "status": "Completed",
            "descriptionForAdmins": "Test",
            "descriptionForReviewers": "Test",
            "createdBy": {
                "id": "36c4c56e-fce3-4e2d-b28e-4ac0c7d2fa10",
                "displayName": "MOD Administrator",
                "userPrincipalName": "admin@contoso.com"
            },
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
                "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null,
                "inactiveDuration": "P30D"
            },
            "instanceEnumerationScope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            },
            "reviewers": [
                {
                    "query": "./owners",
                    "queryType": "MicrosoftGraph",
                    "queryRoot": null
                }
            ],
            "backupReviewers": [],
            "fallbackReviewers": [],
            "settings": {
                "mailNotificationsEnabled": true,
                "reminderNotificationsEnabled": true,
                "justificationRequiredOnApproval": true,
                "defaultDecisionEnabled": true,
                "defaultDecision": "Approve",
                "instanceDurationInDays": 3,
                "autoApplyDecisionsEnabled": true,
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
                        "startDate": "2021-04-30",
                        "endDate": "2021-04-30"
                    }
                },
                "applyActions": [
                    {
                        "@odata.type": "#microsoft.graph.removeAccessApplyAction"
                    }
                ]
            },
            "instances": []
        }
    ]
}
```
